----------------------------------------------------
DFD Dictionary
----------------------------------------------------
----------------------------------------------------
Entities:
----------------------------------------------------

Corporate Developer - Internal employees in charge of developing, maintaining and integrating, internal, proprietary, as well as external, open source code. To be used in any software or project, for internal or external use, by the company.

Project Manager - A manager directly overseeing the related development project, This person is responsible for the project and all its parts including; risk, OS use, funding, etc.

----------------------------------------------------
Data Stores:
----------------------------------------------------

SPDX DB - This contains the viability, SPDX manifests, and the approved or allowed usage of any piece of open source code a developer wishes to integrate into a project.

Policy DB - This contains all the policy information.

NIST CPE Information - This is a local copy of all the current CPEs from the National Vulnerabilities Database.

----------------------------------------------------
Processes:
----------------------------------------------------

Policy Information - Process that checks and verifys policy within the database.

Manage Project Information - This process provides the Corporate Manager with file/package information about the project.

Manage CPE Information - A process in chich CPE request is sent to the National Vulnaribility Database and the received information is stored in NIST CPE Database

Version Control - Process which allows the developer to check in and manage code.

License Scanner - This process provides scans packages or the files for license information.

Code Approval - Corporate Manager approves code and sends it to the developer.

Upload code to website - Developer takes code and uploads to website.

----------------------------------------------------
Data Flows:
----------------------------------------------------

File/Package: A single file or a collection of files in a package.

Project File: A single file containing code.

License Information: Information returned about the licenses within the file/package.

CPE Information: Contains all CPE information from the National Vulnerability Database.

Package Name: The name of the package that is/was submitted by the developer.

CVE Information :It is the information used to find vulnerabilities in packages.

File SHA1 Request: A request, using a hash to see if a file already exists in the database.

File SHA1 Response: A "yes" or "no" response from the database to confirm or deny the presence of the file in the database.

Project Information Request: Request sent by the corporate manager for project information from the OSS database.

Project Information Response: Response sent back to the corporate manager about project information.

New Policy Information: Submit new policy information by the corporate manager.

Policy Respond: Policy information about the project is returned to the manager.

Project Information Request: The policy database is queried for policy information for the project.

Project Information Response: The policy information for the specific project is returned.

CPE Request: A request for updated CPE information from the National Vulnerability Database.

CPE Response: Updated CPE information is returned.

CVE Request: Information about the CVE of a file/package is requested from the National Vulnerability Database using CPE information.
