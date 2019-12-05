

Administration of registers
---------------------------

Registers of openIMIS serve as a principal tool by which openIMIS is adjusted to needs of health insurance schemes. With exception of the register of Users that can be managed only by users with the system role openIMIS Administrator or with a role including an access to Administration/Users or Locations, all other registers can be managed by users with the role Scheme Administrator.or with a role including an access to Administration/Products or Health Facilities or Pricelists or Medical Services or Medical Items or Enrolment Officers or Claim Administrators or Payer. There is no system role that includes an access to the register of user profiles. Only users having a role including an access to Administration/User Profiles can access the register of User Profiles.

The register of Users defines who can login to openIMIS and under what constraints. The register of Locations defines administrative division of the territory, on which a health insurance scheme is operated. The register of Payers allows specification of institutional payers that can pay contributions on behalf of policy holders (households, groups of persons). The register of Enrolment Agents specifies all persons (either employed or contracted) by the scheme administration that are entitled to distribute/sell policies to population. The register of Claim Administrators specifies all employees of health facilities that are entitled to submit claims to the scheme administration. The register of Health Facilities contains all contractual health facilities that can submit claims to the scheme administration. The register of Medical Items specifies all possible medical items (drugs, prostheses, medical devices etc.) that can be used in definitions of packages of insurance products and in pricelists associated with contractual health facilities. The register of Pricelists that splits into two divisions for Medical Services and for Medical Items contains pricelists valid for individual health facilities or their groups reflecting results of price negotiations between contractual health facilities and the scheme administration. Finally, the register of Products includes definitions of all insurance products that can be distributed/ sold within the health insurance scheme.


.. toctree::
   :maxdepth: 3

   product
   health_facility
   medical_service
   medical_item
   service_price_list
   item_price_list
   user
   user_roles
   enrolment_officer
   claim_admin
   payer
   location