Derived operational indicators report
-------------------------------------

  The report provides operational indicators derived from primary operational indicators. The report can be run by users with the system role Manager or with a role including an access to Tools/Reports/Derived Operational Indicators. The table below will provide an overview on the actual derived indicators provided by the report.
  
  #. Parameters for selection for the report:

    .. _image207:
    .. figure:: /img/user_manual/image176.png
      :align: center

      `Image 207 - Derived Operational Indicators Report Criteria`

  #. Input parameters of the report:

    * Month– the period  in which a payment takes place

    * Year  - the period  in which a payment takes place – **mandatory**

    * Region – region of activity of enrolment officers 

    * District - District of activity of enrolment officers

    * Insurance Product – the drop down list with available insurance products for the district according to standard IMIS rules - **mandatory** 

    * HF code - the drop down list with available HF products for the District according to standard IMIS rules

    
  #. The title of the report

    * Region 
    
    * District - District if one selected

    * Insurance Product

    * HF code 


  #. Content of the report

    .. list-table:: Table Overview of derived operational indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable

        * - **Code**
          - **Derived**
          - **Dimension**
          - **Description**

        * - D1
          - Incurred claims ratio
          - Time, Insurance product
          - It is the ratio P11/P9

        * - D2
          - Renewal ratio
          - Time, Insurance product
          - It is the ratio P5/P4

        * - D3
          - Growth ratio
          - Time, Insurance product
          - It is the ratio P2/P1-for immediately preceding period

        * - D4
          - Promptness of claims settlement
          - Time, Insurance product
          - It is the average (date of sending to payment- Date of submission of the claim) for all claims relating to given insurance product and emerging in a respective period Date of sending of payment is not in the structure of Claim, it has to be retrieved from a journal-can be?)

        * - D5
          - Claims settlement ratio
          - Time, Health facility, Insurance product
          - It is the ratio (P10-P12)/P10

        * - D6
          - Number of claims per insuree
          - Time, Insurance product
          - It is the ratio P10/P6

        * - D7
          - Average cost per claim
          - Time, Health facility, Insurance product
          - It is the ratio P11/P10

        * - D8
          - Satisfaction level
          - TimeDistrict, Health facility
          - The average mark from feedbacks received in a respective period

        * - D9
          - Feedback response ratio
          - Time, District, Health facility
          - The ratio of number of feedbacks received (up to time of creation of the report) and number of feedbacks asked for in a respective period

  #. Example

    .. _image227:
    .. figure:: /img/user_manual/image195.png
      :align: center

      `Image 227 - Preview – Derived Operational Indicators Report`
