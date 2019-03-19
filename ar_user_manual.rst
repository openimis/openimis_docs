
Analytic and reporting user manual
==================================

The Analytic and Reporting component of the Insurance Management Information System (AR-IMIS) provides managerial data for management of health insurance schemes supported by IMIS, allows easy and speedy analysis of these data with the objective to reveal causes of different phenomena encountered in supported health insurance schemes. Provided data allow also monitoring of developments within supported health insurance schemes and identification of potential errors in operational data.

Concept of AR-IMIS
^^^^^^^^^^^^^^^^^^

The concept of AR-IMIS is based on populating of the Data Warehouse with aggregate data from the operational database of IMIS. This populating is done automatically and regularly (usually once a week) from the operational database by Extract, Transformation and Loading process (ETL). Within this process data from the operational database are aggregated and stored in the Data Warehouse in conformance with multidimensional data model (:ref:`image271`).

.. _image271:
.. figure:: /img/user_manual/image236.png
  :align: center

  `Image 271 - Concept of AR-IMIS`

This model is suitable for analysis of data. Questions like “What is the number of newly covered insurees by an insurance product at during a calendar period and who were of an age, a gender, lived in a location and were cared for by a Enrolment officer? Data in the multidimensional Data Warehouse are presented by a suitable front-end tool. Currently AR-IMIS uses MS Excel as the front-end presentation tool. An Excel file is remotely connected to the Data Warehouse and data are stored in the Excel file in the form of so called pivot tables. The multidimensional model is based on the notion of facts and dimensions. The facts (indicators) are what we are interested in. For example, a fact may number of insured persons, number of active policies, number of submitted claims etc. Facts can be looked at from different angles-for example from the point of view of age and gender of insured persons, from the point of view of time period etc. These angles (points of view) are captured by the notion of dimensions that are used for qualification of facts (:ref:`image272`).

.. _image272:
.. figure:: /img/user_manual/image237.png
  :align: center

  `Image 272 - Facts and dimensions`

A dimension is composed from points that represent specific values in the dimension for which we want to look at facts-for example *November* 2015 may be one point in the Time dimension. Points of a dimension may be organized in hierarchies. Higher levels of hierarchies represent more aggregate views. Going to the lower levels by so called *drill down* operation we can analyze facts in more detail-for example we may drill down from calendar years to quarters of corresponding calendar years and further to months. We can go in an opposite direction and look at facts from more aggregate points of view (*drill up*).For example from looking at the amount of collected contributions in calendar months we can look at the same indicator according to quarters of a year or according to calendar years.

..

Facts with related meaning and the identical set of qualifying dimension are represented in the multidimensional model of the Data Warehouse as so called cubes. We can do other operations on cubes as for example *slicing* when we select one or several points in one dimension and look at the rest of cube or dicing when we select on or several points in two or more dimensions. All such operations allow analysis of data in the Data Warehouse in an easy and comprehensive way.

Dimensions
^^^^^^^^^^

Dimensions represent our point of view on facts. Each dimension has several values (points). The points are used for qualification of our view on the facts. AR-IMIS provides values of facts corresponding to specified points across one or more dimensions. The points may be organized in hierarchies. Lower levels of a hierarchy allow looking at a fact according to more specific points. For example, the most important *Time* dimension has at the lowest level calendar months. The calendar months are grouped into quarters and quarters into calendar years. So, we can get a value of a fact corresponding to a specific month. Going one level up in the dimension *Time*, we can get can get a value of the fact corresponding to a specific quarter and going even up we can get a value of the fact corresponding to a specific calendar year. If we don’t specify any point in a dimension, it means we are interested in a value of a fact for all points together in the given dimension.

..

AR-IMIS defines several dimensions. Their meaning is dependent on the context of a fact for which they are used. For example, for the fact *Number of submitted claims* the *Time* dimension means in AR-IMIS a period in which claimed health care was provided. It could have also other interpretations, for example, it may be a period in which claims were submitted. Exact interpretation of each dimension is indicated with description of each fact provided below.

..

The points of a dimension are either fixed, e.g. the points *Sex* are *Male/Female/Undefined* for the dimension, or are obtained from registers in the operational part of IMIS. For example, the points for the dimension *Services* are obtained from the current status of the register of services in IMIS.

..

The following table shows dimensions used across AR-IMIS. For each dimension its name, names of attributes used for referencing of their points, source for their points, and their meaning.

.. |lk_loc_reg| replace:: `register of locations`_
.. _`register of locations` : web_app_vb_user_manual.html#locations-administration

.. |lk_ins_reg| replace:: `register of insurance products`_
.. _`register of insurance products` : web_app_vb_user_manual.html#insurance-products-administration

.. |lk_pay_reg| replace:: `register of payers`_
.. _`register of payers` : web_app_vb_user_manual.html#payers-administration

.. |lk_off_reg| replace:: `register of enrolment officers`_
.. _`register of enrolment officers` : web_app_vb_user_manual.html#enrolment-officers-administration

.. |lk_ser_reg| replace:: `register of medical services`_
.. _`register of medical services` : web_app_vb_user_manual.html#medical-services-administration

.. |lk_itm_reg| replace:: `register of medical items`_
.. _`register of medical items` : web_app_vb_user_manual.html#medical-items-administration

.. |lk_dia_reg| replace:: `list of diagnoses`_
.. _`list of diagnoses` : web_app_vb_user_manual.html#upload-list-of-diagnoses

.. |lk_hfa_reg| replace:: `register of health facilities`_
.. _`register of health facilities` : web_app_vb_user_manual.html#health-facilities-administration

+-----------------+-----------------+-----------------+-----------------+
|         Name    | Names of        | Source of data  | Points          |
|                 | hierarchy /     |                 |                 |
|                 | attributes      |                 |                 |
+=================+=================+=================+=================+
| **Time**        | Time Hierarchy  | generated by    | Hierarchy:      |
|                 |                 | openIMIS        |                 |
|                 | **Other         |                 | Years->Quarters |
|                 | fields**:       |                 | ->Months        |
|                 |                 |                 |                 |
|                 | Month Name      |                 |                 |
|                 |                 |                 |                 |
|                 | Quarter Name    |                 |                 |
|                 |                 |                 |                 |
|                 | Year Time       |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Age**         | Age Range       | generated by    | below1,1-4,5-9… |
|                 |                 | openIMIS        | ,               |
|                 |                 |                 | 80+,Unkown      |
+-----------------+-----------------+-----------------+-----------------+
| **Gender**      | Gender Name     | generated by    | Male, Female,   |
|                 |                 | openIMIS        | Unknown         |
+-----------------+-----------------+-----------------+-----------------+
| **Regions**     | Region          | |lk_loc_reg|    | Hierarchy:      |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 | Regions->Distri |
|                 | **Other         |                 | cts->Wards->Vil |
|                 | fields**:       |                 | lages           |
|                 |                 |                 |                 |
|                 | Region          |                 |                 |
|                 |                 |                 |                 |
|                 | District        |                 |                 |
|                 |                 |                 |                 |
|                 | Ward            |                 |                 |
|                 |                 |                 |                 |
|                 | Village         |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Products**    | Product         | |lk_ins_reg|    | Hierarchy:      |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 | Regions->Distri |
|                 | **Other         |                 | cts->Products   |
|                 | fields**:       |                 |                 |
|                 |                 |                 |                 |
|                 | Region          |                 |                 |
|                 |                 |                 |                 |
|                 | District        |                 |                 |
|                 |                 |                 |                 |
|                 | Product Name    |                 |                 |
|                 |                 |                 |                 |
|                 | Product Code    |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Payers**      | Payer Name      | |lk_pay_reg|    | Families,       |
|                 |                 |                 | Payers (the     |
|                 |                 |                 | list of)        |
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Officers**    | Officer         | |lk_off_reg|    | Hierarchy:      |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 | Regions->Distri |
|                 | **Other         |                 | cts->Enrolment  |
|                 | fields**:       |                 | Officers        |
|                 |                 |                 |                 |
|                 | Region          |                 |                 |
|                 |                 |                 |                 |
|                 | District        |                 |                 |
|                 |                 |                 |                 |
|                 | Last Name       |                 |                 |
|                 |                 |                 |                 |
|                 | Other Names     |                 |                 |
|                 |                 |                 |                 |
|                 | Assistant Code  |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Services**    | Service         | |lk_ser_reg|    | Hierarchy:      |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 | (Curative,      |
|                 | **Other         |                 | Preventive)->Se |
|                 | fields**:       |                 | rvices          |
|                 |                 |                 |                 |
|                 | Service Code    |                 |                 |
|                 |                 |                 |                 |
|                 | Service Name    |                 |                 |
|                 |                 |                 |                 |
|                 | Service         |                 |                 |
|                 | Category        |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Items**       | Item Hierarchy  | |lk_itm_reg|    | Hierarchy:      |
|                 |                 |                 |                 |
|                 | **Other         |                 | (Drugs,         |
|                 | fields**:       |                 | Prostheses)->It |
|                 |                 |                 | ems             |
|                 | Item Code       |                 |                 |
|                 |                 |                 |                 |
|                 | Item Name       |                 |                 |
|                 |                 |                 |                 |
|                 | Item Category   |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Diseases**    | Disease         | |lk_dia_reg|    |                 |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 |                 |
|                 | **Other         |                 |                 |
|                 | fields**:       |                 |                 |
|                 |                 |                 |                 |
|                 | Disease Name    |                 |                 |
|                 |                 |                 |                 |
|                 | Disease Code    |                 |                 |
|                 |                 |                 |                 |
|                 | Disease         |                 |                 |
|                 | Category        |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Providers**   | Provider        | |lk_hfa_reg|    | Hierarchy:      |
|                 | Hierarchy       |                 |                 |
|                 |                 |                 | Regions->Distri |
|                 | **Other         |                 | cts->           |
|                 | fields**:       |                 | (Dispensary,    |
|                 |                 |                 | Health Centre,  |
|                 | Provider Name   |                 | Hospital)       |
|                 |                 |                 | ->Health        |
|                 | Disease Code    |                 | facility        |
|                 |                 |                 |                 |
|                 | Provider        |                 |                 |
|                 | Category        |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| **Care          | Category Care   | generated by    | Emergency,      |
| Category**      |                 | openIMIS        | Other,          |
|                 |                 |                 | Referral,       |
|                 |                 |                 | Unknown         |
+-----------------+-----------------+-----------------+-----------------+
| **Care Type**   | Care Type       | generated by    | In-patient,     |
|                 |                 | openIMIS        | Out-patient,    |
|                 |                 |                 | Unknown         |
+-----------------+-----------------+-----------------+-----------------+
| **Questions**   | Question        | generated by    | Care Rendered,  |
|                 |                 | openIMIS        | Drug            |
|                 |                 |                 | Prescribed,     |
|                 |                 |                 | Drug Received,  |
|                 |                 |                 | Payment Aske,   |
|                 |                 |                 | Unknown         |
+-----------------+-----------------+-----------------+-----------------+

`Table 9.1 Overview of dimensions`


Facts
^^^^^

Facts provided by AR-IMIS can be structured into the areas according to (:ref:`image273`). Within each area several facts packed into one or several cubes are provided. Facts are packed into the same cube if they have an associated meaning and are provided with the same set of dimension. The following articles lists available cubes according to the areas, for each cube indicates available facts with description of their meaning and

.. _image273:
.. figure:: /img/user_manual/image238.png
  :align: center

  `Image 273 - Areas of facts`

underlying set of qualifying dimensions. If meaning of a dimension is not straightforward, its description is provided. It relates especially to the *Time* dimension where it is important which datum related with a fact is taken as the governing date for association with given point (period) in the *Time* dimension.

Facts on Enrolment and policies
"""""""""""""""""""""""""""""""

This group of facts relates to acquisition of insures and development of coverage by health insurance schemes. Facts available are listed in `Table 9.2 <#table-9.2-facts-on-Enrolment-and-policies>`__

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Population  | Population  | Number of   | Gender      |             |
|             |             | inhabitants |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Region      |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+
| Number of   | Number of   | Number of   | Region      |             |
| families/gr | families/gr | households  |             |             |
| oups        | oups        | according   |             |             |
|             |             | to a census |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+
| Current and | Current     | Insurees    | Age         | Age at the  |
| new         | insurees    | covered by  |             | end of a    |
| insurees    |             | at least    |             | time period |
|             |             | one policy  |             |             |
|             |             | active at   |             |             |
|             |             | the end of  |             |             |
|             |             | a time      |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Enrolment   | An          |
|             |             |             | Officers    | Enrolment   |
|             |             |             |             | officer     |
|             |             |             |             | responsible |
|             |             |             |             | for         |
|             |             |             |             | correspondi |
|             |             |             |             | ng          |
|             |             |             |             | policy      |
|             +-------------+-------------+-------------+-------------+
|             | New         | Insurees    | Region      | Place of    |
|             | acquired    | newly       |             | living of a |
|             | insurees    | insured     |             | household   |
|             |             | during a    |             |             |
|             |             | time period |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    | An          |
|             |             |             |             | insurance   |
|             |             |             |             | product     |
|             |             |             |             | covering an |
|             |             |             |             | insuree     |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Period of   |
|             |             |             |             | Enrolment   |
|             |             |             |             | of insurees |
|             |             |             |             | for new     |
|             |             |             |             | insurees    |
|             |             |             |             |             |
|             |             |             |             | Period of   |
|             |             |             |             | effective   |
|             |             |             |             | day and     |
|             |             |             |             | later of    |
|             |             |             |             | their       |
|             |             |             |             | policies    |
|             |             |             |             | for current |
|             |             |             |             | insurees    |
+-------------+-------------+-------------+-------------+-------------+
| All types   | Current     | Number of   | Age         | Age of the  |
| of policies | policies    | active      |             | head of a   |
|             |             | policies at |             | household   |
|             |             | the end of  |             | at the end  |
|             |             | a time      |             | of a time   |
|             |             | period      |             | period      |
|             +-------------+-------------+-------------+-------------+
|             | Expired     | Number of   | Gender      | Gender of   |
|             | policies    | policies    |             | the head of |
|             |             | that        |             | a household |
|             |             | expired     |             |             |
|             |             | during a    |             |             |
|             |             | time period |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Renewed     | Number of   | Enrolment   | An          |
|             | policies    | policies    | Officers    | Enrolment   |
|             |             | that were   |             | officer     |
|             |             | renewed     |             | responsible |
|             |             | during a    |             | for         |
|             |             | time period |             | correspondi |
|             |             |             |             | ng          |
|             |             |             |             | policy      |
|             +-------------+-------------+-------------+-------------+
|             | Sold        | Number of   | Region      | Place of    |
|             | policies    | policies    |             | living of a |
|             |             | that were   |             | household   |
|             |             | sold during |             |             |
|             |             | a time      |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    | An          |
|             |             |             |             | insurance   |
|             |             |             |             | product of  |
|             |             |             |             | a policy    |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Period of   |
|             |             |             |             | Enrolment   |
|             |             |             |             | date for    |
|             |             |             |             | sold        |
|             |             |             |             | policies    |
|             |             |             |             |             |
|             |             |             |             | Period of   |
|             |             |             |             | expiry date |
|             |             |             |             | for expired |
|             |             |             |             | policies    |
|             |             |             |             |             |
|             |             |             |             | Period of   |
|             |             |             |             | renewal     |
|             |             |             |             | date(when   |
|             |             |             |             | renewing    |
|             |             |             |             | was done)   |
|             |             |             |             | for renewed |
|             |             |             |             | policies    |
|             |             |             |             |             |
|             |             |             |             | Period of   |
|             |             |             |             | effective   |
|             |             |             |             | day and     |
|             |             |             |             | later for   |
|             |             |             |             | current     |
|             |             |             |             | policies    |
+-------------+-------------+-------------+-------------+-------------+
| Share of    | Share of    | =Current    | Gender      |             |
| insured     | insured     | insures /   |             |             |
| population  | population  | Population  |             |             |
|             |             |             |             |             |
|             |             | at the end  |             |             |
|             |             | of a time   |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Region      | Place of    |
|             |             |             |             | living of a |
|             |             |             |             | household   |
|             |             |             +-------------+-------------+
|             |             |             | Products    | An          |
|             |             |             |             | insurance   |
|             |             |             |             | product     |
|             |             |             |             | covering an |
|             |             |             |             | insuree     |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+
| Share of    | Number of   | Number of   | Region      | Place of    |
| insured     | insured     | households  |             | living of a |
| families/gr | families/gr | that are    |             | household   |
| oups        | oups        | covered by  |             |             |
|             |             | at least    |             |             |
|             |             | one active  |             |             |
|             |             | policy at   |             |             |
|             |             | the end of  |             |             |
|             |             | a time      |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+
|             | Share of    | =Number of  | Region      | Place of    |
|             | insured     | insured     |             | living of a |
|             | families/gr | households  |             | household   |
|             | oups        | /Number of  |             |             |
|             |             | households  |             |             |
|             |             |             |             |             |
|             |             | at the end  |             |             |
|             |             | of a time   |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.2 Facts on Enrolment and policies`

Facts on collected revenue
""""""""""""""""""""""""""

This group of facts relates to revenue of health insurance schemes. Facts available are listed in `Table 9.3 <\l>`__.

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Contributio | Contributio | Contributio | Enrolment   | Collection  |
| n           | n           | ns          | Officers    | of          |
| collection  | collected   | collected   |             | contributio |
|             |             | in given    |             | ns          |
|             |             | time period |             | from        |
|             |             |             |             | policies of |
|             |             |             |             | an          |
|             |             |             |             | Enrolment   |
|             |             |             |             | officer     |
|             |             |             +-------------+-------------+
|             |             |             | Payers      | Collection  |
|             |             |             |             | of          |
|             |             |             |             | contributio |
|             |             |             |             | ns          |
|             |             |             |             | from an     |
|             |             |             |             | institution |
|             |             |             |             | al          |
|             |             |             |             | payer or    |
|             |             |             |             | from        |
|             |             |             |             | families    |
|             |             |             |             | itself      |
|             |             |             +-------------+-------------+
|             |             |             | Products    | Collection  |
|             |             |             |             | of          |
|             |             |             |             | contributio |
|             |             |             |             | ns          |
|             |             |             |             | within an   |
|             |             |             |             | insurance   |
|             |             |             |             | product     |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Period of   |
|             |             |             |             | payment     |
|             |             |             |             | date of     |
|             |             |             |             | contributio |
|             |             |             |             | ns          |
+-------------+-------------+-------------+-------------+-------------+
| Contributio | Contributio | Amount of   | Products    | Allocation  |
| n           | n           | collected   |             | of          |
| allocation  | allocated   | contributio |             | contributio |
|             |             | ns          |             | ns          |
|             |             | allocated   |             | within an   |
|             |             | proportiona |             | insurance   |
|             |             | lly         |             | product     |
|             |             | for using   |             |             |
|             |             | in a time   |             |             |
|             |             | period      |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Period of   |
|             |             |             |             | allocation  |
|             |             |             |             | of          |
|             |             |             |             | contributio |
|             |             |             |             | ns          |
|             |             |             +-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.3 Facts on contributions`

Facts on claims
"""""""""""""""

This group of facts relates to claims forwarded by health care providers to administrators of health insurance schemes. Facts available are listed in `Table 9.4 <#table-9.4-facts-on-claims>`__.

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Claim       | Amount      | Total       | Providers   | Providers   |
| details     | claimed     | amount in   |             | that        |
|             |             | nominal     |             | entered and |
|             |             | prices that |             | or          |
|             |             | was         |             | submitted   |
|             |             | submitted   |             | claims      |
|             |             | by health   |             |             |
|             |             | care        |             |             |
|             |             | providers   |             |             |
|             |             | for health  |             |             |
|             |             | care        |             |             |
|             |             | provided in |             |             |
|             |             | given       |             |             |
|             |             | period      |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Amount      | Total       | Time        | Time period |
|             | rejected    | amount that |             | of          |
|             |             | was on      |             | provision   |
|             |             | totally     |             | of health   |
|             |             | rejected    |             | care that   |
|             |             | claims      |             | was         |
|             |             |             |             | invoiced in |
|             |             |             |             | claims      |
|             +-------------+-------------+-------------+-------------+
|             | Entered     | Number of   |             |             |
|             | claims      | claims      |             |             |
|             |             | entered     |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Submitted   | Number of   |             |             |
|             | claims      | claims      |             |             |
|             |             | submitted   |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Rejected    | Number of   |             |             |
|             | claims      | claims      |             |             |
|             |             | totally     |             |             |
|             |             | rejected    |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Average     | =Amount     |             |             |
|             | amount      | claimed/    |             |             |
|             | claimed     | Submitted   |             |             |
|             |             | claims      |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Average     | =Amount     |             |             |
|             | amount      | rejected/   |             |             |
|             | rejected    | Rejected    |             |             |
|             |             | claims      |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Claim       | Amount      | Amount      | Providers   | Providers   |
| details     | adjusted    | adjusted    |             | that        |
| products    |             | after       |             | submitted   |
|             |             | processing  |             | claims      |
|             |             | in nominal  |             |             |
|             |             | prices      |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Amount paid | Amount      | Products    | Products by |
|             |             | actually to |             | which       |
|             |             | be paid to  |             | health care |
|             |             | health      |             | claimed was |
|             |             | facilities  |             | covered     |
|             |             | taking into |             |             |
|             |             | account     |             |             |
|             |             | indexes of  |             |             |
|             |             | relative    |             |             |
|             |             | pricing     |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Processed   | Number of   | Time        | Time period |
|             | claims      | claims sent |             | of          |
|             |             | for         |             | provision   |
|             |             | valuation   |             | of health   |
|             |             |             |             | care that   |
|             |             |             |             | was         |
|             |             |             |             | invoiced in |
|             |             |             |             | claims      |
|             +-------------+-------------+-------------+-------------+
|             | Paid claims | Number of   |             |             |
|             |             | claims      |             |             |
|             |             | actually    |             |             |
|             |             | valuated    |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Average     | =Amount     |             |             |
|             | amount      | adjusted/Pr |             |             |
|             | adjusted    | ocessed     |             |             |
|             |             | claims      |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Average     | =Amount     |             |             |
|             | amount paid | paid/       |             |             |
|             |             | Valuated    |             |             |
|             |             | claims      |             |             |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.4 Facts on claims`

Facts on utilization of health care
"""""""""""""""""""""""""""""""""""

This group of facts relates to utilization of health care by insures according to submitted and not rejected claims. Facts available are listed in `Table 9.5 <#table-9.5-facts-on-of-utilization-health-care>`__

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Admissions  | Number of   | Number of   | Age         | Age at the  |
| and visits  | hospital    | hospital    |             | time of     |
| and         | admissions  | admissions  |             | provision   |
| hospital    |             |             |             | health care |
| days        |             |             |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             +-------------+-------------+-------------+-------------+
|             | Number of   |             | Care        |             |
|             | hospital    |             | category    |             |
|             | days        |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | Average     | = Number of | Products    | In case two |
|             | length of   | hospital    |             | or more     |
|             | stay        | days/       |             | insurance   |
|             |             | Number of   |             | products    |
|             |             | hospital    |             | covered a   |
|             |             | admissions  |             | hospital    |
|             |             |             |             | admission/v |
|             |             |             |             | isit,       |
|             |             |             |             | it is       |
|             |             |             |             | accounted   |
|             |             |             |             | to each of  |
|             |             |             |             | them        |
+-------------+-------------+-------------+-------------+-------------+
|             | Number of   |             | Providers   | Providers   |
|             | out-patient |             |             | which       |
|             | visits      |             |             | claimed     |
|             |             |             |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Utilization | Services    | Number of   | Age         | Age at the  |
| of services | utilized    | utilized    |             | time of     |
|             |             | services    |             | provision   |
|             |             | according   |             | health care |
|             |             | to          |             |             |
|             |             | submitted   |             |             |
|             |             | claims.     |             |             |
|             |             |             |             |             |
|             |             | If a        |             |             |
|             |             | service was |             |             |
|             |             | provided    |             |             |
|             |             | during one  |             |             |
|             |             | visit/hospi |             |             |
|             |             | tal         |             |             |
|             |             | stay, the   |             |             |
|             |             | service is  |             |             |
|             |             | counted     |             |             |
|             |             | according   |             |             |
|             |             | to the      |             |             |
|             |             | number of   |             |             |
|             |             | its         |             |             |
|             |             | provision   |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Care        |             |
|             |             |             | category    |             |
|             |             |             +-------------+-------------+
|             |             |             | Care type   |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Providers   | Providers   |
|             |             |             |             | which       |
|             |             |             |             | claimed     |
|             |             |             |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Services    |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Utilization | Items       | Number of   | Age         | Age at the  |
| of medical  | utilized    | utilized    |             | time of     |
| items       |             | medical     |             | provision   |
|             |             | items       |             | health care |
|             |             | according   |             |             |
|             |             | to          |             |             |
|             |             | submitted   |             |             |
|             |             | claims      |             |             |
|             |             |             |             |             |
|             |             | If a        |             |             |
|             |             | medical     |             |             |
|             |             | item was    |             |             |
|             |             | provided    |             |             |
|             |             | during one  |             |             |
|             |             | visit/hospi |             |             |
|             |             | tal         |             |             |
|             |             | stay, the   |             |             |
|             |             | medical     |             |             |
|             |             | item is     |             |             |
|             |             | counted     |             |             |
|             |             | according   |             |             |
|             |             | to the      |             |             |
|             |             | number of   |             |             |
|             |             | its         |             |             |
|             |             | provision   |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Care        |             |
|             |             |             | category    |             |
|             |             |             +-------------+-------------+
|             |             |             | Care type   |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Providers   | Providers   |
|             |             |             |             | which       |
|             |             |             |             | claimed     |
|             |             |             |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Items       |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Average     | Average     | = Services  | Age         | Age at the  |
| utilization | utilization | utilized /  |             | time of     |
| of services | of services | Current     |             | provision   |
| per insuree | per insuree | insurees    |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Services    |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Average     | Average     | = Items     | Age         |             |
| utilization | utilization | utilized /  |             |             |
| of medical  | of medical  | Current     |             |             |
| items per   | items per   | insurees    |             |             |
| insuree     | insuree     |             |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Items       |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        |             |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.5 Facts on of utilization health care`

Facts on expenditures for health care
"""""""""""""""""""""""""""""""""""""

This group of facts relates to expenditures for health care actually paid to health care providers. Facts available are listed in `Table 9.6 <#table-9.6-facts-on-expenditures-for-health-care>`__

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Expenditure | Service     | Expenditure | Age         | Age at the  |
| s           | expenditure | s           |             | time of     |
| for         | s           | for         |             | provision   |
| services    |             | services    |             | health care |
|             |             | actually    |             |             |
|             |             | remunerated |             |             |
|             |             | to health   |             |             |
|             |             | facilities  |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Care        |             |
|             |             |             | category    |             |
|             |             |             +-------------+-------------+
|             |             |             | Care type   |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Providers   | Providers   |
|             |             |             |             | which       |
|             |             |             |             | claimed     |
|             |             |             |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Services    |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Expenditure | Item        | Expenditure | Age         | Age at the  |
| s           | expenditure | s           |             | time of     |
| for medical | s           | for medical |             | provision   |
| items       |             | items       |             | health care |
|             |             | actually    |             |             |
|             |             | remunerated |             |             |
|             |             | to health   |             |             |
|             |             | facilities  |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Care        |             |
|             |             |             | category    |             |
|             |             |             +-------------+-------------+
|             |             |             | Care type   |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Providers   | Providers   |
|             |             |             |             | which       |
|             |             |             |             | claimed     |
|             |             |             |             | health care |
|             |             |             +-------------+-------------+
|             |             |             | Items       |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Average     | Average     | = Service   | Age         | Age at the  |
| expenditure | expenditure | expenditure |             | time of     |
| s           | s           | s/          |             | provision   |
| for         | for         | Current     |             | health care |
| services    | services    | insurees    |             |             |
| per insuree | per insuree |             |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Services    |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Average     | Average     | = Item      | Age         | Age at the  |
| expenditure | expenditure | expenditure |             | time of     |
| s           | s           | s/          |             | provision   |
| for medical | for medical | Number of   |             | health care |
| items per   | items per   | inhabitants |             |             |
| insuree     | insuree     |             |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     | .           |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Items       |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+
| Average     | Average     | = Average   | Age         | Age at the  |
| expenditure | expenditure | expenditure |             | time of     |
| s           | s           | s           |             | provision   |
| for health  | per insuree | of services |             | health care |
| care per    |             | per insuree |             |             |
| insuree     |             | + Average   |             |             |
|             |             | expenditure |             |             |
|             |             | s           |             |             |
|             |             | for medical |             |             |
|             |             | items per   |             |             |
|             |             | insuree     |             |             |
|             |             |             +-------------+-------------+
|             |             |             | Gender      |             |
|             |             |             +-------------+-------------+
|             |             |             | Disease     |             |
|             |             |             +-------------+-------------+
|             |             |             | Products    |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Hospital    |
|             |             |             |             | admissions  |
|             |             |             |             | are         |
|             |             |             |             | associated  |
|             |             |             |             | with time   |
|             |             |             |             | periods     |
|             |             |             |             | according   |
|             |             |             |             | to dates of |
|             |             |             |             | discharge.  |
|             |             |             |             | Time period |
|             |             |             |             | of          |
|             |             |             |             | provision   |
|             |             |             |             | of health   |
|             |             |             |             | care        |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.6 Facts on expenditures for health care`

Facts on feedbacks
""""""""""""""""""

This group of facts relates to evaluation of request for feedbacks on provided health care that are issued by medical officers during processing of claims. Facts available are listed in `Table 9.7 <\l>`__

+-------------+-------------+-------------+-------------+-------------+
| Cube        | Fact        | Meaning     | Dimension   | Comment     |
+=============+=============+=============+=============+=============+
| Feedback    | Feedbacks   | Number of   | Products    | Insurance   |
| details     | sent        | requests    |             | products    |
|             |             | for         |             | that        |
|             |             | feedbacks   |             | covered     |
|             |             | sent in a   |             | claims      |
|             |             | time period |             | initiating  |
|             |             |             |             | requests    |
|             |             |             |             | for         |
|             |             |             |             | feedbacks   |
|             +-------------+-------------+-------------+-------------+
|             | Feedbacks   | Number of   | Providers   | Providers   |
|             | responded   | feedbacks   |             | that        |
|             |             | received in |             | submitted   |
|             |             | a time      |             | claims      |
|             |             | period      |             | initiating  |
|             |             |             |             | requests    |
|             |             |             |             | for         |
|             |             |             |             | feedbacks   |
|             +-------------+-------------+-------------+-------------+
|             | Overall     | Sum of all  | Time        | Period of   |
|             | assessment  | assessment  |             | sending/rec |
|             |             | overall     |             | eiving      |
|             |             | assessment  |             | feedbacks   |
|             |             | marks in    |             |             |
|             |             | responded   |             |             |
|             |             | feedbacks   |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Feedback    | = Feedbacks |             |             |
|             | return      | responded/  |             |             |
|             | share       | Feedbacks   |             |             |
|             |             | sent        |             |             |
|             +-------------+-------------+-------------+-------------+
|             | Average     | = Overall   |             |             |
|             | overall     | assessment/ |             |             |
|             | assessment  | Feedbacks   |             |             |
|             |             | responded   |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Feedback    | Answers Yes | Count of    | Products    | Insurance   |
| answers     |             | all Yes     |             | products    |
|             |             | answers     |             | that        |
|             |             |             |             | covered     |
|             |             |             |             | claims      |
|             |             |             |             | initiating  |
|             |             |             |             | requests    |
|             |             |             |             | for         |
|             |             |             |             | feedbacks   |
|             +-------------+-------------+-------------+-------------+
|             | Share of    | = Answers   | Providers   | Providers   |
|             | Answers Yes | Yes/        |             | that        |
|             |             | Feedbacks   |             | submitted   |
|             |             | responded   |             | claims      |
|             |             |             |             | initiating  |
|             |             |             |             | requests    |
|             |             |             |             | for         |
|             |             |             |             | feedbacks   |
|             |             |             +-------------+-------------+
|             |             |             | Questions   |             |
|             |             |             +-------------+-------------+
|             |             |             | Time        | Period of   |
|             |             |             |             | sending/rec |
|             |             |             |             | eiving      |
|             |             |             |             | feedbacks   |
+-------------+-------------+-------------+-------------+-------------+

`Table 9.7 Facts on feedbacks`

How access data from the Data Warehouse
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Data from the Data Warehouse can be accessed by means of an Excel file. As access to the Data Warehouse is protected, a user has to get from an administrator of AR-MIS URL of the Data Warehouse for remote access, a userid and a password. A userid may allow access to all data in the Data Warehouse or only to a subset of data corresponding to a specific region, to selected regions, to a specific district or to selected districts.

..

The procedure of accessing of data is as follows (:ref:`image274`)

.. _image274:
.. figure:: /img/user_manual/image239.png
  :align: center

  `Image 274 - Accessing the Data Warehouse`

1. Open an Excel file

2. Click on the menu item **Data**

3. Click on the sub-menu **From Other Sources**

4. Click on the sub-menu **From Analysis Services**

5. A dialog box appears for specification of logon data:

   a. Enter URL of the Data Warehouse into the field **Server Name**

   b. Select the option **Use the following user name and password**

   c. Enter your userid into the field **User Name**

   d. Enter your password into the field **Password**

   e. Click on **Finish**

6. A box appears (**Select Database and Tables**) with the list of available cubes. Select one and click on **Finish**

7. A box appears (**Save Data Connection File and Finish**).Check the box **Save passport in file** and click on **Finish**.

8. A box appears (**Import Data**). Select whether cube should be accessed by a pivot table and/or chart and specify a placement of the pivot table. Click on **OK**.

9. An area for the pivot table appears in the sheet with the **Pivot Table Field** area on the right (:ref:`image274`). Click on facts to be displayed and click or drag dimensions to appropriate sectors of the pivot table in the **Pivot Table Field** area.

  .. _image275:
  .. figure:: /img/user_manual/image240.png
    :align: center

    `Image 275 - Pivot Table in Excel`
