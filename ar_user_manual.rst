
Analytic and reporting user manual
==================================

  The Analytic and Reporting component of the Insurance Management Information System (AR-IMIS) provides managerial data for management of health insurance schemes supported by IMIS, allows easy and speedy analysis of these data with the objective to reveal causes of different phenomena encountered in supported health insurance schemes. Provided data allow also monitoring of developments within supported health insurance schemes and identification of potential errors in operational data.

Concept of AR-IMIS
^^^^^^^^^^^^^^^^^^

  The concept of AR-IMIS is based on populating of the Data Warehouse with aggregate data from the operational database of IMIS. This populating is done automatically and regularly (usually once a week) from the operational database by Extract, Transformation and Loading process (ETL). Within this process data from the operational database are aggregated and stored in the Data Warehouse in conformance with multidimensional data model (:ref:`image271`).

  .. _image271:
  .. figure:: /img / user_manual / image236.png
    :align: center

    `Image 271 - Concept of AR-IMIS`

  This model is suitable for analysis of data. Questions like “What is the number of newly covered insurees by an insurance product at during a calendar period and who were of an age, a gender, lived in a location and were cared for by a Enrolment officer? Data in the multidimensional Data Warehouse are presented by a suitable front-end tool. Currently AR-IMIS uses MS Excel as the front-end presentation tool. An Excel file is remotely connected to the Data Warehouse and data are stored in the Excel file in the form of so called pivot tables. The multidimensional model is based on the notion of facts and dimensions. The facts (indicators) are what we are interested in. For example, a fact may number of insured persons, number of active policies, number of submitted claims etc. Facts can be looked at from different angles-for example from the point of view of age and gender of insured persons, from the point of view of time period etc. These angles (points of view) are captured by the notion of dimensions that are used for qualification of facts (:ref:`image272`).

  .. _image272:
  .. figure:: /img / user_manual / image237.png
    :align: center

    `Image 272 - Facts and dimensions`

  A dimension is composed from points that represent specific values in the dimension for which we want to look at facts-for example *November* 2015 may be one point in the Time dimension. Points of a dimension may be organized in hierarchies. Higher levels of hierarchies represent more aggregate views. Going to the lower levels by so called *drill down* operation we can analyze facts in more detail-for example we may drill down from calendar years to quarters of corresponding calendar years and further to months. We can go in an opposite direction and look at facts from more aggregate points of view (*drill up*).For example from looking at the amount of collected contributions in calendar months we can look at the same indicator according to quarters of a year or according to calendar years.


  Facts with related meaning and the identical set of qualifying dimension are represented in the multidimensional model of the Data Warehouse as so called cubes. We can do other operations on cubes as for example *slicing* when we select one or several points in one dimension and look at the rest of cube or dicing when we select on or several points in two or more dimensions. All such operations allow analysis of data in the Data Warehouse in an easy and comprehensive way.

Dimensions
^^^^^^^^^^

  Dimensions represent our point of view on facts. Each dimension has several values (points). The points are used for qualification of our view on the facts. AR-IMIS provides values of facts corresponding to specified points across one or more dimensions. The points may be organized in hierarchies. Lower levels of a hierarchy allow looking at a fact according to more specific points. For example, the most important *Time* dimension has at the lowest level calendar months. The calendar months are grouped into quarters and quarters into calendar years. So, we can get a value of a fact corresponding to a specific month. Going one level up in the dimension *Time*, we can get can get a value of the fact corresponding to a specific quarter and going even up we can get a value of the fact corresponding to a specific calendar year. If we don’t specify any point in a dimension, it means we are interested in a value of a fact for all points together in the given dimension.


  AR-IMIS defines several dimensions. Their meaning is dependent on the context of a fact for which they are used. For example, for the fact *Number of submitted claims* the *Time* dimension means in AR-IMIS a period in which claimed health care was provided. It could have also other interpretations, for example, it may be a period in which claims were submitted. Exact interpretation of each dimension is indicated with description of each fact provided below.


  The points of a dimension are either fixed, e.g. the points *Sex* are *Male / Female / Undefined* for the dimension, or are obtained from registers in the operational part of IMIS. For example, the points for the dimension *Services* are obtained from the current status of the register of services in IMIS.


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

  .. list-table:: `Table 9.1 Overview of dimensions`
      :widths: 2 3 4 2
      :header-rows: 1
      :stub-columns: 1
      :class: longtable

      * - **Name**
        - **Names of hierarchy / attributes**
        - **Source of data**
        - **Points**

      * - **Time**
        - | * Month
          | * Quarter
          | * Year
        - generated by openIMIS
        - Hierarchy: Years ->Quarters ->Months

      * - **Age**
        - Age Range
        - generated by openIMIS
        - below1, 80+ ...

      * - **Gender**
        - Gender Name
        - generated by openIMIS
        - Male Unknown

      * - **Regions**
        - | * Region
          | * District
          | * Ward
          | * Village
        - |lk_loc_reg|
        - Hierarchy: Regions->Districts ->Wards ->Villages

      * - **Products**
        - | * Region
          | * District
          | * Product Name
          | * Product Code
        - |lk_ins_reg|
        - Hierarchy: Regions ->Districts ->Products

      * - **Payers**
        - Payer Name
        - |lk_pay_reg|
        - Families Payers (the list of)


      * - **Officers**
        - | * Region
          | * District
          | * Last Name
          | * Other name
          | * Assistant Code
        - |lk_off_reg|
        - Hierarchy: Regions ->Districts ->Enrolment Officers

      * - **Services**
        - | * Service Code
          | * Service Name
          | * Service Category
        - |lk_ser_reg|
        - Hierarchy: (Curative Preventive) ->Services

      * - **Items**
        - | * Item Code
          | * Item Name
          | * Item Category
        - |lk_itm_reg|
        - Hierarchy: (Drugs Prostheses) ->Items

      * - **Diseases**
        - | * Disease Code
          | * Disease Name
          | * Disease Category
        - |lk_dia_reg|
        -

      * - **Providers**
        - | * Provider Code
          | * Provider Name
          | * Provider Category
        - |lk_hfa_reg|
        - Hierarchy: Regions ->Districts ->(Dispensary Health Centre Hospital) ->Health facility

      * - **Care Category**
        - Category Care
        - generated by openIMIS
        - Emergency Other Referral Unknown

      * - **Care Type**
        - Care Type
        - generated by openIMIS
        - In-patient Out-patient Unknown

      * - **Questions**
        - Question
        - generated by openIMIS
        - Care Rendered Drug Prescribed Drug Received Payment Aske Unknown


Facts
^^^^^

  Facts provided by AR-IMIS can be structured into the areas according to (:ref:`image273`). Within each area several facts packed into one or several cubes are provided. Facts are packed into the same cube if they have an associated meaning and are provided with the same set of dimension. The following articles lists available cubes according to the areas, for each cube indicates available facts with description of their meaning and

  .. _image273:
  .. figure:: /img / user_manual / image238.png
    :align: center

    `Image 273 - Areas of facts`

  underlying set of qualifying dimensions. If meaning of a dimension is not straightforward, its description is provided. It relates especially to the *Time* dimension where it is important which datum related with a fact is taken as the governing date for association with given point (period) in the *Time* dimension.

Facts on Enrolment and policies
"""""""""""""""""""""""""""""""

  This group of facts relates to acquisition of insures and development of coverage by health insurance schemes. Facts available are listed in `Table 9.2 <#table-9.2-facts-on-Enrolment-and-policies>`__

  .. list-table:: `Table 9.2 Facts on Enrolment and policies`
      :widths: 2 2 4 2 4
      :header-rows: 1
      :stub-columns: 1
      :class: longtable

      * - **Cube**
        - **Fact**
        - **Meaning**
        - **Dimension**
        - **Comment**

      * - Population
        - Population
        - Number of inhabitants
        - Gender
        -

      * -
        -
        -
        - Region
        -

      * -
        -
        -
        - Time
        -

      * - Number of families / groups
        - Number of families / groups
        - Number of households according to a census
        - Region
        -

      * -
        -
        -
        - Time
        -

      * - Current and new insurees
        - Current insurees
        - Insurees covered by at least one policy active at the end of a time period
        - Age
        - Age at the end of a time period

      * -
        -
        -
        - Gender
        -

      * -
        -
        -
        - Enrolment Officers
        - An enrolment officer responsible for corresponding policy

      * -
        - New acquired insurees
        - Insurees newly insured during a time period
        - Region
        - Place of living of a household

      * -
        -
        -
        - Products
        - An insurance product covering an insuree

      * -
        -
        -
        - Time
        - Period of enrolment of insurees for new insurees Period of effective day and later of their policies for current insurees

      * - All types of policies
        - Current policies
        - Number of active policies at the end of a time period
        - Age
        - Age of the head of a household at the end of a time period

      * -
        - Expired policies
        - Number of policies that expired during a time period
        - Gender
        - Gender of the head of a household

      * -
        - Renewed policies
        - Number of policies that were renewed during a time period
        - Enrolment Officers
        - An enrolment officer responsible for corresponding policy

      * -
        - Sold policies
        - Number of policies that were sold during a time period
        - Region
        - Place of living of a household

      * -
        -
        -
        - Products
        - An insurance product of a policy

      * -
        -
        -
        - Time
        - Period of enrolment date for sold policies Period of expiry date for expired policies Period of renewal date(when renewing was done)  for renewed policies Period of effective day and later for current policies

      * - Share of insured population
        - Share of insured population
        - Current insures /  Population at the end of a time period
        - Gender
        -

      * -
        -
        -
        - Region
        - Place of living of a household

      * -
        -
        -
        - Products
        - An insurance product covering an insuree

      * -
        -
        -
        - Time
        -

      * - Share of insured families / groups
        - Number of insured families / groups
        - Number of households that are covered by at least one active policy at the end of a time period
        - Region
        - Place of living of a household

      * -
        -
        -
        - Time
        -

      * -
        - Share of insured families / groups
        - =Number of insured households / Number of households at the end of a time period
        - Region
        - Place of living of a household

      * -
        -
        -
        - Time
        -


Facts on collected revenue
""""""""""""""""""""""""""

  This group of facts relates to revenue of health insurance schemes. Facts available are listed in `Table 9.3 <\l>`__.

  .. list-table:: `Table 9.3 Facts on contributions`
    :widths: 2 2 4 2 4
    :header-rows: 1
    :stub-columns: 1
    :class: longtable

    * - **Cube**
      - **Fact**
      - **Meaning**
      - **Dimension**
      - **Comment**

    * - Contribution collection
      - Contribution collected
      - contributions collected in given time period
      - Enrolment Officers
      - Collection of contributions from policies of an enrolment officer

    * -
      -
      -
      - Payers
      - Collection of contributions from an institution al payer or from families itself

    * -
      -
      -
      - Products
      - Collection of contributions within an insurance product

    * -
      -
      -
      - Time
      - Period of payment date of contributions

    * - Contribution allocation
      - Contribution allocated
      - Amount of collected contributions allocated proportionally for using in a time period
      - Products
      - Allocation of contributions within an insurance product

    * -
      -
      -
      - Time
      - Period of allocation of contributions


Facts on claims
"""""""""""""""

  This group of facts relates to claims forwarded by health care providers to administrators of health insurance schemes. Facts available are listed in `Table 9.4 <#table-9.4-facts-on-claims>`__.

  .. list-table:: `Table 9.4 Facts on claims`
    :widths: 2 2 4 2 4
    :header-rows: 1
    :stub-columns: 1
    :class: longtable

    * - **Cube**
      - **Fact**
      - **Meaning**
      - **Dimension**
      - **Comment**

    * - Claim details
      - Amount claimed
      - Total amount in nominal prices that was submitted by health care providers for health care provided in given period
      - Providers
      - Providers that entered and or submitted claims

    * -
      - Amount rejected
      - Total amount that was on totally rejected claims
      - Time
      - Time period of provision of health care that was invoiced in claims

    * -
      - Entered claims
      - Number of claims entered
      -
      -

    * -
      - Submitted claims
      - Number of claims submitted
      -
      -

    * -
      - Rejected claims
      - Number of claims totally rejected
      -
      -

    * -
      - Average amount claimed
      - =Amount claimed / Submitted claims
      -
      -

    * -
      - Average amount rejected
      - =Amount rejected / Rejected claims
      -
      -

    * - Claim details products
      - Amount adjusted
      - Amount adjusted after processing in nominal prices
      - Providers
      - Providers that submitted claims

    * -
      - Amount paid
      - Amount actually to be paid to health facilities taking into account indexes of relative pricing
      - Products
      - Products by which health care claimed was covered

    * -
      - Processed claims
      - Number of claims sent for valuation
      - Time
      - Time period of provision of health care that was invoiced in claims

    * -
      - Paid claims
      - Number of claims actually valuated
      -
      -

    * -
      - Average amount adjusted
      - =Amount adjusted / Pr ocessed claims
      -
      -

    * -
      - Average amount paid
      - =Amount paid/ Valuated claims
      -
      -


Facts on utilization of health care
"""""""""""""""""""""""""""""""""""

  This group of facts relates to utilization of health care by insures according to submitted and not rejected claims. Facts available are listed in `Table 9.5 <#table-9.5-facts-on-of-utilization-health-care>`__

.. list-table:: `Table 9.5 Facts on of utilization health care`
    :widths: 2 2 4 2 4
    :header-rows: 1
    :stub-columns: 1
    :class: longtable

    * - **Cube**
      - **Fact**
      - **Meaning**
      - **Dimension**
      - **Comment**

    * - Admissions and visits and hospital days
      - Number of hospital admissions
      - Number of hospital admissions
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      - Number of hospital days
      -
      - Care category
      -

    * -
      - Average length of stay
      - = Number of hospital days / Number of hospital admissions
      - Products
      - In case two or more insurance products covered a hospital admission / visit, it is accounted to each of them

    * -
      - Number of out-patient visits
      -
      - Providers
      - Providers which claimed health care

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Utilization of services
      - Services utilized
      - | Number of utilized services according to submitted claims.
        | If a service was provided during one visit / hospital stay, the service is counted according to the number of its provision
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Care category
      -

    * -
      -
      -
      - Care type
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Providers
      - Providers which claimed health care

    * -
      -
      -
      - Services
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Utilization of medical items
      - Items utilized
      - | Number of utilized medical items according to submitted claims
        | If a medical item was provided during one visit / hospital stay, the medical item is counted according to the number of its provision
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Care category
      -

    * -
      -
      -
      - Care type
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Providers
      - Providers which claimed health care

    * -
      -
      -
      - Items
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Average utilization of services per insuree
      - Average utilization of services per insuree
      - = Services utilized / Current insurees
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Services
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Average utilization of medical items per insuree
      - Average utilization of medical items per insuree
      - = Items utilized / Current insurees
      - Age
      -

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Items
      -

    * -
      -
      -
      - Time
      -

Facts on expenditures for health care
"""""""""""""""""""""""""""""""""""""

  This group of facts relates to expenditures for health care actually paid to health care providers. Facts available are listed in `Table 9.6 <#table-9.6-facts-on-expenditures-for-health-care>`__

 .. list-table:: `Table 9.6 Facts on expenditures for health care`
    :widths: 2 2 4 2 4
    :header-rows: 1
    :stub-columns: 1
    :class: longtable

    * - **Cube**
      - **Fact**
      - **Meaning**
      - **Dimension**
      - **Comment**

    * - expenditures for services
      - Service expenditures
      - Expenditures for services actually remunerated to health facilities
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Care category
      -

    * -
      -
      -
      - Care type
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Providers
      - Providers which claimed health care

    * -
      -
      -
      - Services
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - expenditures for medical items
      - Item expenditures
      - expenditures for medical items actually remunerated to health facilities
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Care category
      -

    * -
      -
      -
      - Care type
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Providers
      - Providers which claimed health care

    * -
      -
      -
      - Items
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Average expenditures for services per insuree
      - Average expenditures for services per insuree
      - = Service expenditures/ Current insurees
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Services
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Average expenditures for medical items per insuree
      - Average expenditures for medical items per insuree
      - = Item expenditures/ Number of inhabitants
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Items
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

    * - Average expenditures for health care per insuree
      - Average expenditures per insuree
      - = Average expenditures of services per insuree + Average expenditures for medical items per insuree
      - Age
      - Age at the time of provision health care

    * -
      -
      -
      - Gender
      -

    * -
      -
      -
      - Disease
      -

    * -
      -
      -
      - Products
      -

    * -
      -
      -
      - Time
      - Hospital admissions are associated with time periods according to dates of discharge. Time period of provision of health care

Facts on feedbacks
""""""""""""""""""

  This group of facts relates to evaluation of request for feedbacks on provided health care that are issued by medical officers during processing of claims. Facts available are listed in `Table 9.7 <\l>`__

  .. list-table:: `Table 9.7 Facts on feedbacks`
    :widths: 2 2 4 2 4
    :header-rows: 1
    :stub-columns: 1
    :class: longtable

    * - **Cube**
      - **Fact**
      - **Meaning**
      - **Dimension**
      - **Comment**

    * - Feedback details
      - Feedbacks sent
      - Number of requests for feedbacks sent in a time period
      - Products
      - Insurance products that covered claims initiating requests for feedbacks

    * -
      - Feedbacks responded
      - Number of feedbacks received in a time period
      - Providers
      - Providers that submitted claims initiating requests for feedbacks

    * -
      - Overall assessment
      - Sum of all assessment overall assessment marks in responded feedbacks
      - Time
      - Period of sending / rec eiving feedbacks

    * -
      - Feedback return share
      - = Feedbacks responded/ Feedbacks sent
      -
      -

    * -
      - Average overall assessment
      - = Overall assessment/ Feedbacks responded
      -
      -

    * - Feedback answers
      - Answers Yes
      - Count of all Yes answers
      - Products
      - Insurance products that covered claims initiating requests for feedbacks

    * -
      - Share of Answers Yes
      - = Answers Yes/ Feedbacks responded
      - Providers
      - Providers that submitted claims initiating requests for feedbacks

    * -
      -
      -
      - Questions
      -

    * -
      -
      -
      - Time
      - Period of sending / receiving feedbacks


How access data from the Data Warehouse
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  Data from the Data Warehouse can be accessed by means of an Excel file. As access to the Data Warehouse is protected, a user has to get from an administrator of AR-MIS URL of the Data Warehouse for remote access, a userid and a password. A userid may allow access to all data in the Data Warehouse or only to a subset of data corresponding to a specific region, to selected regions, to a specific district or to selected districts.


  The procedure of accessing of data is as follows (:ref:`image274`)

  .. _image274:
  .. figure:: /img / user_manual / image239.png
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

  8. A box appears (**Import Data**). Select whether cube should be accessed by a pivot table and / or chart and specify a placement of the pivot table. Click on **OK**.

  9. An area for the pivot table appears in the sheet with the **Pivot Table Field** area on the right (:ref:`image274`). Click on facts to be displayed and click or drag dimensions to appropriate sectors of the pivot table in the **Pivot Table Field** area.

    .. _image275:
    .. figure:: /img / user_manual / image240.png
       :align: center

       `Image 275 - Pivot Table in Excel`
