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

Text here

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
