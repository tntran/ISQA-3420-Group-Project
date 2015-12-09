Case 1:

      Title: Determine License and Vulnerability Information 

      Primary Actor: Corporate Manager

      Goal in Context: The corporate manager is able to determine license and vulnerability information from provided project   information

      Stakeholders:

      -Corporate Manager: To receive clear and relevant project information
      -Corporate Developer: To provide the relevant file/package level information 
      -Project Owner: To clearly understand corporate manager decisions to green/red light a project 
 
      Preconditions: 

     -Relevant file/package information is in the SPDX database
     -Proper project information has been provided
     
     Main Success Scenario: Corporate manager receives accurate license and vulnerability information for the requested project   packages
    
    Failed End Conditions: Corporate manager receives inaccurate or invalid license and vulnerability information for the
    requested project packages

     Trigger: Corporate manager uploads or identifies project information to which license and vulnerability information is  provided



Case 2:

     Title: Verify external source code license information

     Primary Actor: Corporate Developer

     Goal in Context : Developer manager will be able to verify the license on the external source code to be incorporate in     the project source code

     Stakeholders:

    -Corporate Developer: To provide the source code file/package information
    -Corporate Manager: to receive clear and relevant source code license information
    -Project Owner: To clearly understand corporate manager decisions to incorporate the source code.

     Preconditions :

    -Proper project information has been provided
    -External source code file/package must follow project guide line and requirement
    -Relevant license information is in the SPDX database

     Main Success Scenario: Developer manager receives appropriate and accurate license information on the external source code     for the requested project packages.

     Failed End Conditions: License information failed to meet the project guide line; or manager received inaccurate and     invalid incense information for the project.

     Trigger: Developer manager uploads or identifies the external source code license information to which license was       verified.



Case 3:

      Title: Obtain CPE information 

      Primary Actor: Corporate Developer

      Goal in Context: The corporate developer is able to obtain CPE information from the National Vulnerability database and store it in NIST CPE data store.

      Stakeholders:

     -Corporate Manager: To receive clear and relevant project information
     -Corporate Developer: To provide the relevant file/package level information 
     -Project Owner: To clearly understand corporate manager decisions to green/red light a project 
 
     Preconditions:

    -Relevant file/package information is in the National Vulnerability Database database
    -Proper file/project information is provided.  

     Main Success Scenario: Corporate developer receives accurate CPE information information for the requested files/packages

     Failed End Conditions: Corporate developer receives inaccurate or invalid CPE information for the requested project packages

     Trigger: Corporate manager uploads or identifies files for which CPE information is required.
