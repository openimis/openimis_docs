Claim History Report
--------------------



    The Claim Overview report is an essential tool for communication between an insurer and health facilities. This report assumes that a health facility is given and all claims according to other specific criteria are included in the report.

    The required Claim History report is very similar to the Claim Overview report but it is centred around a given insuree. All claims belonging to an insuree according to other specific criteria are included in the Claim History report. The way of displaying of claims is similar to the Claim Overview report

  #. Parameters for selection for the report:

    .. _lcy_reports_flt_ch:
    .. figure:: /img/user_manual/lcy_reports_flt_ch.png
      :align: center

      `Claim History Report`

  #. Input parameters of the report:

    * Date From -the start date of period, in which a visit was accomplished or a discharge took place-obligatory

    * Date To- the end date of the period –obligatory

    * Region – the region of health facilities for which the claim history should be included

    * District– the district  of health facilities for which the claim history should be included

    * Insurance Product – the insurance product for which the claim history should be included

    * Health Facility-the health facility for which the claim history should be included

    * Insurance Number- the insurance number of an insure(patient) for whom the claim history should be included - obligatory

    * Claim Status –the status of claims that should be included in the report (from a drop down list of possible states of a claim)

    * Scope-the level of details that are included with a claim in the report (Claims Only, Claims and Rejection Details, Claims and All Details – see RfC 95)

  
  #. The title of the report

    See Input paramaters

    * Date From  - first claim date to be considered in the report **Mandatory**

    * Date To  - last claim date to be considered in the report **Mandatory**

    * Region – if it was entered

    * District –if it was entered

    * Health Facility (the code and the name)- if it was entered

    * Insurance product (the code and the name)-if it was entered

    * Scope  (claim only, Claims and rejection details, Claimn and all details)

    * Claim Status (Entered, Checked, Processed, Valuated, Rejected)

    * Insurance number, the name of the insuree (Other Name, Last Name) and his/her birth date **Mandatory**

  #. Content of the report

    The report contains the list of items with the following structure:

      * If a region, a district or specific health facility are not entered in the corresponding input parameter then claims displayed are broken down according to these attributes in sections:

        * Region

        * District

        * Health facility (the code and the name)

      * If an attribute given above is entered the corresponding section is missing ( and the parameter is moved into the title of the whole report).
        Example: If only a region is given the claim history relates only to health facilities in the region. The region is in the title of the report and the body of the report is split into sections:

          * District

          * Health facility (the code and the name)

    At the bottom of the report the total number of rejected photos in the report is included.
  
  #. Example


    .. _lcy_reports_ch:
    .. figure:: /img/user_manual/lcy_reports_ch.png
      :align: center

      `Claim History Report`

   




    