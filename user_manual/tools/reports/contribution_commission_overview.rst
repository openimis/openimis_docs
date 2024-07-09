Overview of Commissions
-----------------------

  The report Overview of Commissions summarizes prescribed/actually paid contributions for newly enrolled/renewed policies for families/groups.

  #. Parameters for selection for the report:

    .. _lcy_reports_flt_oca:
    .. figure:: /img/user_manual/lcy_reports_flt_oca.png
      :align: center

      `Overview of Capitation Report Criteria`

  #. Input parameters of the report:

    * Month– the period  in which a payment takes place-obligatory

    * Year  - the period  in which a payment takes place –obligatory

    * Region – region of activity of enrolment officers -obligatory

    * District - region of activity of enrolment officers -obligatory

    * Insurance Product – the drop down list with available insurance products for the district according to standard IMIS rules-optional

    * Enrolment Officer - the drop down list with acting enrolment officers in the district  - optional

    * Payer-a drop down list with available payers according to standard IMIS rules  -optional

    * Mode – a drop down list with the following modes:

      * Prescribed Contributions

      * Actually Paid Contributions

    * Scope-a drop down list with the following scopes:

      * Overview

      * All details

    * Commission Rate – a percentage for calculation of commissions depending on the mode

  #. The title of the report:

    * Mode

    * Commission Rate

    * Period (Month/Year)

    * Region and District

    * Insurance Product ( the code and the name of an insurance product) if specified in the input parameters

    * Enrolment Officer ( the code and the name of an enrolment officer)  if specified in the input parameters

  #. Content of the report

    The report takes into account policies satisfying the following conditions:

    * mode Prescribed Contributions:

      * The policy is activated (it is active now or it will be active in future)

      * The last contribution for the policy was prescribed within the specified period ((Month/Year)

    * mode Actually Paid Contributions:

      * The policy is activated (it is active now or it will be active in future)

      * he last payment of contribution for the policy meets or exceeds the last prescribed contribution and it was matched by the payment module within the specified period ((Month/Year)

  #. Structuring of the report

    Overview Scope

      The report is structured in rows dedicated to an enrolment officer and an insurance product. Each row contains the following data items:

        * Enrolment officer code

        * Enrolment officer name ( Other names +Last name)

        * Phone Number (for the enrolment officer taken  from the register of enrolment officers)

        * Insurance product code

        * Insurance product name

        * Number of policies

        * Amount of contributions

        * Commissions

      Remark 1: if an enrolment officer provides policies of different insurance products then there are several consecutive rows devoted to the enrolment officer according to individual insurance products

      Remark 2: Amount of contributions is the amount of prescribed contribution for the mode Prescribed Contributions and the amount of actually paid (matched) contributions for the mode Actually Paid Contributions.

      The report ends with the following totals:

        * Total number of policies

        * Total amount of contributions

        * Total amount of commissions


    All details scope

      The policies are structured in the following way:

        * If a specific enrolment officer is not specified in the corresponding input parameter the policies are structured in sections  (with the sub-tile the code and the name of an enrolment officer)  according to enrolment officers

        * If a specific insurance product is not specified in the corresponding input parameter the policies are structured in sections  (with the sub-tile the code and the name of an insurance product) according to insurance products

        * If neither  a specific insurance product  nor a specific enrolment officer is not specified in the corresponding input parameter the policies are structured first  in sections   (with the sub-tile the code and the name of an enrolment officer)  according to enrolment officers and within them in sub-sections (with the sub-tile the code and the name of an insurance product) according to insurance products

      Each section/sub section provides the following totals at its end:

        * The total number of  the listed policies in the section/sub-section

        * The total of all prescribed contributions of the listed policies

        * The total of all actual payments of contributions of the listed policies

        * The calculated commission as a product of the Commission Rate and the total of all prescribed contributions

      For each policy the following data items are included in the report:


        * Insurance number of the head of the  family

        * Full name of the head of the family

         * Date of enrolment/renewal of the policy

        * Date of prescribed contribution

        * Receipt code of the prescribed contribution

        * Amount of contribution

        * List of all matched actual payments of the prescribed contribution (transaction number of payment, date of receiving of the payment, actual amount of payment)


        Remark: If a family/group has several policies satisfying the criteria of inclusion in the report or such policies are included separately.

      The following totals are provided at the end of the report:

        * The total number of  the listed policies

        * The total of all prescribed contributions of the listed policies

        * The total of all actual payments of contributions of the listed policies

        * The calculated commission as a product of the Commission Rate and the total of all prescribed contributions

  #. Example


