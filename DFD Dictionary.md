
![alt tag] (https://cloud.githubusercontent.com/assets/16200170/11699209/d335fa48-9e88-11e5-8389-5ad445a64650.png)

External Entities / Externals
Label:

	EXT 1 – Tenant

Description:

	Tenant request for apartment leasing from the company.
________________________________________
Label:

	EXT 2 – Manager

Description:

	The manager process and assign tenant new apartment.

Data Flows
  
Context Diagram
Label:

	DAF 6 – Tenant Request

Description:

Tenant Request is used to apply for apartment.

Decomposition:
Tenant Name =
	First Name +
	(Middle Initial) +
	Last Name
Tenant Address =
	Street + 
	(Apartment) +
	City +
	State +
	Zip +
	Country

Apartment Information=
Category+
Price
Apartment Status=
Newly Fix+
	Upgrade+
	Require Update+
	Require Replacement+
	Damage+
Manager Name=
	First Name +
	(Middle Initial) +
	Last Name
Manager Property=
	Apartment Location+
	Location Condition+
	
![alt tag](https://cloud.githubusercontent.com/assets/16200170/11699237/05c919fe-9e89-11e5-88d0-846535d1696f.png)



Level 0 Diagram


Process 1.0

Label:

	PRC 1 – Determine Tenant Background

Description:

This process describes the specific steps check tenant background.

Decomposition

	RECEIVE Tenant Request from Tenant
	CHECK Tenant Information 
BEGIN IF 
IF Tenant Information = New
	THEN 
SEND Tenant Information to Background Checking
		ELSE
			SEND Tenant Information to PRC 2
		ENDIF
	ENDIF
	READ Tenant Information from Tenant table
	WRITE New Tenant Information to Tenant table
	


![alt tag](https://cloud.githubusercontent.com/assets/16200170/11699250/13e5ca82-9e89-11e5-94ee-99f5e919403f.png)
PRC 2

Label:

	PRC 2.0 – Approve and Assign Apartment

Description:

This process determines whether the Tenant get approve and assign a new apartment.

Decomposition:

REVIEW New Tenant Information from PRC 1.0
READ the Apartment Status from Apartment table
BEGIN IF
	IF 
Apartment = available
	THEN
		SEND Assign Apartment to Tenant	
	ELSE
		SEND Denied Notification to Tenant
ENDIF
WRITE New Apartment Approval to Apartment Table
	

Label:

	DAF 8 – Apartment Status	

Description:

This process determines whether the apartment are available for lease.

Decomposition:

Apartment Status=
Newly Fix+
	Upgrade+
	Require Update+
	Require Replacement+
	Damage+
	


PRC 3.0

Label:

	PRC 3.0 – Review Report Request

Description:

The process generates the Report to Manager.

Decomposition:

REVIEW Tenant Information from PRC 2.0 
VERIFY Apartment Information from Apartment
GENERATE Report for Manager
	SEND Tenant Information and Apartment Information to Managers
	


 


Level-1 PRC 1.1

Label:

	PRC 1.1 – Check Tenant Background

Description:

The process check tenant background.

Decomposition:

RECEIVE Tenant Request from Tenant
	READ Tenant Information from Tenant table
	BEGIN IF
		IF Tenant Information = New Tenant Information
		THEN SEND Tenant Information through Determine Background
		ELSE REJECT Tenant Information from Tenant
END IF
WRITE New Tenant Information to Tenant table


	
 


Level-1 PRC 1.2

Label:

	PRC 1.1 – Apartment Assign

Description:

The process assign apartment for approve tenant.

Decomposition:

RECEIVE New Tenant Information from Tenant table
BEGIN IF
		IF New Tenant Information= Approval
		THEN Assign Apartment to Tenant
		ELSE SEND Denied to Tenant
END IF
SEND Apartment New Information to Apartment
