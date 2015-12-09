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

     Title: Policy Check

     Primary Actor: Corporate Manager

     Goal in Context : Corporate Manager has the ability to examine policy documents and compare them to the given manifest.

     Stakeholders:

    -Corporate Developer: To receive a positive report for the documents being compared.
    -Corporate Manager: To verify the information provided is clear.

     Preconditions :

    -Proper policy document has been provided
    -A manifest containing license and vulnerability information is provided for the managers use.

     Main Success Scenario: The corporate manager compares and checks documents within the policy database.

     Failed End Conditions: The varified information between the project and document fails to meet the policy check.

     Trigger: Corporate manager collects and updates the vulnerability and license information.



Case 3:

      Title: Obtain New software system 

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
