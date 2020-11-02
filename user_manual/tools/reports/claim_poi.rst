Primary operational indicators  - claims report
-----------------------------------------------

    The report provides aggregate data relating to policies and insurees according to insurance products. The report can be run by users with the system role Manager or with a role including an access to Tools/Reports/Primary Operational Indicators-claims. The table below will provide an overview on   primary indicators of the report.

  #. Parameters for selection for the report:

    .. _image206:
    .. figure:: /img/user_manual/lcy_reports_flt_poic.png
      :align: center

      `Image 206 - Primary Operational Indicators - Claims Report Criteria`

  #. Input parameters of the report:

    * Month– the period  in which a payment takes place

    * Quarter  - the period  in which a payment takes place 

    * Year  - the period  in which a payment takes place – **mandatory**

    * Region – region of activity of enrolment officers 

    * District - region of activity of enrolment officers

    * Insurance Product – the drop down list with available insurance products for the district according to standard IMIS rules - **mandatory** 

  
  #. The title of the report

    See Input paramaters

  #. Content of the report

  #. Structuring of the report
  
    .. list-table:: Table Overview of operational indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable

        * - **Code**
          - **Primary indicators**
          - **Dimension**
          - **Description**

        * - P10
          - Number of claims
          - Time, Health facility, Insurance product
          - The number of claims for given insurance product that emerged during a respective period (Start dateof a claim is within the respective period)

        * - P11
          - Amount remunerated
          - Time, Health facility, Insurance product
          - Amount remuneratedfor claims for given insurance product that emerged during a respective period (Start dateof a claim is within the respective period)

        * - P12
          - Number of rejected claims
          - Time, Health facility, Insurance product
          - The number of claims for given insurance product that emerged during a respective period and were rejected (Start dateof a claim is within the respective period and the Status approval ofthe claim is Rejected)

  #. Example

    .. _image226:
    .. figure:: /img/user_manual/image194.png
      :align: center

      `Image 226 - Preview – Primary Operational Indicators - Claims Report`
