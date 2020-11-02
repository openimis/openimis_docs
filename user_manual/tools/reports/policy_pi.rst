Primary operational indicators  - policies report
-------------------------------------------------

  The report provides aggregate data relating to policies and insurees according to insurance products. The report can be run by users with the system role Manager or with a role including an access to Tools/Reports/Primary Operational Indicators-policies. The table below will provide an overview on   primary indicators of the report.
  
  #. Parameters for selection for the report:

      .. _image205:
      .. figure:: /img/user_manual/image174.png
        :align: center

        `Image 205 - Primary Operational Indicators - Policies Report Criteria`
  
  #. Input parameters of the report:

    * Month– the period  in which a payment takes place

    * Quarter  - the period  in which a payment takes place 

    * Year  - the period  in which a payment takes place – **mandatory**

    * Region – region of activity of enrolment officers 

    * District - region of activity of enrolment officers

    * Insurance Product – the drop down list with available insurance products for the district according to standard IMIS rules - **mandatory** 

    * HF code - the drop down list with available HF products for the District according to standard IMIS rules

  #. The title of the report

    * Period (Month/Quarter Year)

    * Region and District

    * Insurance Product ( the code and the name of an insurance product) if specified in the input parameters

  #. Content of the report

    .. list-table:: Table  Overview of Policies indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable

        * - **Code**
          - **Primary indicators**
          - **Dimension**
          - **Description**

        * - P1
          - Number of policies
          - Time, Insurance product
          - The number of policies of given insurance product on the last day of a respective period (Status of the policy is Active, the last day of period is within <Effective date, Expiry day>)

        * - P2
          - Number of new policies
          - Time, Insurance product
          - The number of new policies of given insurance product during a respective period (Enrolment date is within the respective period, there is ``no`` preceding policy with the same (or before converted) insurance product forgiven policy)

        * - P3
          - Number of suspended policies
          - Time, Insurance product
          - The number of policies for given insurance product that were suspended during a respective period (Status of the policy is Suspended, suspension took place within the respective period)

        * - P4
          - Number of expired policies
          - Time, Insurance product
          - The number of policies for given insurance product that expired during a respective period (Status of the policy is Expired,expiration took place within the respective period)

        * - P5
          - Number of renewals
          - Time, Insurance product
          - The number of policies that were renewed forgiven insurance product (or a converte done) during a respective period ( Enrolment date is within the respective period, there is a preceding policy with the same (or before converted) product forgiven

        * - P6
          - Number of insurees
          - Time, Insurance product
          - The number of insurees covered by policies of given insurance product on the last day of a respective period (An insuree belongs to a family with an active coverage on the last day of the respective period-see P1 )

        * - P7
          - Number of newly insured insurees
          - Time, Insurance product
          - The number of insurees covered by new policies of given insurance product during a respective period (An insuree belongs to a family with newly acquired policy during the respective period-see P2 )

        * - P8
          - Newly collected Contributions
          - Time, Insurance product
          - Amount of acquired Contributions (for policies of given insurance product) during a respective period ( Date of payment of a Contribution is within the respective period)

        * - P9
          - Available Contributions
          - Time, Insurance product
          - Amount of Contributions that should be allocated for policies of given insurance product for a respective period provided a uniform distribution throughout the insurance period takes place. (If the respective period overlaps with <Effective date, Expiry day> of a policy then a proportional part of corresponding Contributions relating to the respective period is included in available Contributions)


  #. Example

    .. _image225:
    .. figure:: /img/user_manual/image193.png
      :align: center

      `Image 225 - Preview – Primary Operational Indicators - Policies Report`





  
