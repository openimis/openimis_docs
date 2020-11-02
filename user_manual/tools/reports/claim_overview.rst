claim overview
--------------

  The report provides detailed data about results of processing of claims in openIMIS according to insurance products and health facilities. The report can be used as a tool for communication between a health insurance scheme and its contractual health facilities. The report can be run by users with the rsystem role Accountant or with a role including an access to Tools/Reports/Claim Overview. Claims are assigned to the specified period according to date of provision of health care (in case of in-patient care according to the date of discharge).  (:ref:`Image 236<image236>`)


  #. Parameters for selection for the report:

    .. _image217:
    .. figure:: /img/user_manual/image186.png
      :align: center

      `Image 217 - Claim Overview Report Criteria`
  
  #. Input parameters of the report:
  
    * Date From  - first claim date to be considered in the report **Mandatory**

    * Date To  - last claim date to be considered in the report **Mandatory**

    * Region 

    * District 

     * Health Facility (the code and the name)- if it was entered

    * Insurance product (the code and the name)-if it was entered

    * Scope  (claim only, Claims and rejection details, Claimn and all details)

    * Claim Status (Entered, Checked, Processed, Valuated, Rejected)

    * Insuree Number **Mandatory**


  #. The title of the report

    See Input paramaters

  #. Content of the report

    this reports shows the number of claims per hospitals

      * claim only

        * claim code

        * claim date

        * claim admin

        * Visit From

        * Visit To

        * Insurance number

        * Insuree name

        * claim status

        * amount claimed

        * Amount approved

        * Amount adjusted

        * Amount Paid

      * Claims and rejection details:  same as "claim only" plus Rejected Item & service  

        * Item & service code and name

        * Quantity

        * Price

        * Approved Price

        * Justificaiton

        * Valuated

        * Rejection reason

      * Claims and all details:  same as "claim only" plus all Item & service

        * Item & service code and name
        
        * Quantity

        * Price

        * Approved Price

        * Justificaiton

        * Valuated

        * Rejection reason

  
  #. Example

    .. _image236:
    .. figure:: /img/user_manual/image204.png
      :align: center

      `Image 236 Preview – Claim Overview`