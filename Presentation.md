## ISQA 3420 Group Project Presentation

Github Repository: https://github.com/tntran/ISQA-3420-Group-Project

## Members:

Tien Tran 
Evan Schutte 
 
## Slide 1 (Executive Summary)
Problem: Community is vital to an open source community, having a open source license isn't enough to bring together users and developers alone to build a project and community.  Projects start by someone needing to develop a project that intends to meet the need of others. Since  open source code can be used by anyone but need to do that under the license agreement specified within the package. Because there are alot of open source code out there, licences become an important factor to keep 

Solution:  To allow the open source software and code to be legal. The solution for that is to design a better handle the licensing and vulnerabilities. However, this should create a big gap between the campany and the open source community. The system itseft need to 
enable to identify the package information based on the licenses and vulnerabilities. This is not just benefit for the developer but also give credential for the open source community.

## Slide 2 (DFD)

![alt tag](https://cloud.githubusercontent.com/assets/16200170/11701904/19340b7a-9e98-11e5-9600-2cdb46ef2375.png)

## Slide 3 (DFD Dictionary)

## Entities:

Corporate Developer - Internal employees in charge of developing, maintaining and integrating, internal, proprietary, as well as external, open source code. To be used in any software or project, for internal or external use, by the company.

Project Manager - A manager directly overseeing the related development project, This person is responsible for the project and all its parts including; risk, OS use, funding, etc.

## Data Stores:

SPDX DB - This contains the viability, SPDX manifests, and the approved (or allowed) usage of any piece of open source code a developer wishes to integrate into a project.

Policy DB - This contains all the policy information.

NIST CPE Information - This is a local copy of all the current CPEs from the National Vulnerabilities Database.

## Processes:

Policy Information - Process that checks and verifys policy within the database.

Manage Project Information - This process provides the Corporate Manager with file/package information about the project.

Manage CPE Information - A process in chich CPE request is sent to the National Vulnaribility Database and the received information is stored in NIST CPE Database

Version Control - Process which allows the developer to check in and manage code.

License Scanner - This process provides scans packages or the files for license information.

Code Approval - Corporate Manager approves code and sends it to the developer.

Upload code to website - Developer takes code and uploads to website.

## Data Flows:

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

## Slide 4 (ERD)

![alt tag](https://cloud.githubusercontent.com/assets/16200170/11702492/b7c82d80-9e9c-11e5-87c4-05bdc1084c2a.png)

## Slide 5 (Software Manifest)

Document:

      DocumentLicense: CC-BY-SA 4.0
      Author: 
      DateCreated: 
      
Package: 

      Name: 
      SHA1: 
      CPE: 
      Licenses: 
      Vulnerabilities

## Slide 6 (Policy Document)

Licenses:

      Copyleft 
	GPLv2 – Red 
	GPLv3 – Black

      Permissive 
	Apache – Yellow
	MIT – Green 

Vulnerabilities: 

      Scores
	0<X<6 – Yellow
	X>6 – Red 

## Slide 7 (Use Cases)

Case 1:
Title: Determine License and Vulnerability Information 

Primary Actor: Corporate Manager

Goal in Context: The corporate manager is able to determine license and vulnerability information from provided project information

Case 2:
Title: Policy Check

Primary Actor: Corporate Manager

Goal in Context : Corporate Manager has the ability to examine policy documents and compare them to the given manifest.

Case 3:
Title: Upload to Online Repository

Primary Actor: Corporate Developer

Goal in Context: The corporate developer is able to obtain CPE information from the National Vulnerability database and store it in NIST CPE data store.

## Slide 8 (Discuss Experience/Difficulties)

Text here

## Slide 9 (Biggest Takeaways)

Text here
