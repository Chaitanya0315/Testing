
# Project Plan

<!--*This is the template for your project plan. The parts in italics are concise explanations of what should go in the corresponding sections and should not appear in the final document.*-->

**Author**:  Team 47 


**Document Tracking**: Following chart is used to log all the changes made to this document.

| Version | Date of edit/change | Who made the edit/change | Description of edit/change |
| :-----: | :-----------------: | :----------------------: | :------------------------ |
|    v1.0     |    10/06/2017                 |   Team 47                       |           *first draft*                 |
|    v1.1     |    10/20/2017                 |   Team 47                       |           *based on better understanding of the system.*                 |

## 1 Introduction

<!--*Here you introduce the product. Keep this  clean and simple, one or two sentences at most.*-->

The purpose of this group project is to create an android application that will give users a platform to play scramble games, create scramble games, view various player and scramble statistics as well keep track of their own performance.

## 2 Process Description

<!--*Process description as a set of activities; for each activity, provide the following:*-->

<!--- *Activity name (verb or verb phrase)*
- *Activity description (concise paragraph)*
- *Entrance criteria (inputs needed for the activity)*
- *Exit criteria (outputs produced by the activity and how you know it has been completed satisfactorily)*-->

This section illustrates the various activities that team 47 performed throughout the project. These activities are described in terms of the Rational Unified Process (RUP), highlighting all 4 phases that are inception, elaboration, construction, and transition. As per the requirements, each activity has an entrance and an exit criteria. Each document and component pertaining to software development process had various review cycles, resulting in more thorough implementation.


|**STAGE**| **DESCRIPTION**|
|:---:|:---|
|**Inception Stage**| **ACTIVITY [Execution of Project Plan]:** The purpose of this activity was to clearly identify primary tasks which were be accomplished in order to efficiently complete the software development targets. Associating the foreseen objectives with main deliverables and arranging them within different stages of RUP was part of this activity. Primary role assignments amongst the team members based on skill set was also part of this activity.<br><br>**Entrance Criteria**: Understanding the problem statement and following the guidelines of the Rational Unified Process.<br><br>**Exit Criteria**: Acquiring clear knowledge of the project plan which included detailed process explanation and assignment of team roles.<br><br>**ACTIVITY [Use-Case Identification]:** Another major step towards moving the application development process from a concept to a definite design was to clearly understand and interpret the requirements and identifying the actors that shall help the software system to run properly. This activity was responsible for determining the requirements and the major actors involved in completing those requirements. In our case, we had 2 actors, the Player (human) and the External Web Service (system). The output of this activity was the explanation of the initial use-cases in form of a use case diagram accompanied by description of each scenario.<br><br>**Entrance Criteria**: Having a general idea about system and the associated requirements.<br><br>**Exit Criteria**: Creation of the use cases and the use-case diagram. <br><br>**ACTIVITY [System Components Definition]:** Purpose of this activity was to bring into consideration all of the assumptions, constraints and architectural components pertaining to the design identifying the nature of the software system, which in our case in client (Player) - Server (EWS) based. While some of the requirements of the design were clearly specified other additional aspects of the design were illustrated using initial GUI prototypes.<br><br>**Entrance Criteria**: Having better idea about use-case model diagram, system as a whole and program requirements.<br><br>**Exit Criteria**: Generation of the detailed design document containing various design requirements such as deployment diagram, class diagram, component diagram, initial GUI prototype snapshots, etc.|
|**Elaboration Stage**| **ACTIVITY [System Testing Plan]:** The purpose of this activity was be to test the initial level use-case model and the features discussed in the design document. Along with testing for these initial features and use cases, this activity included other essential sub-activities such as bug tracking and overall quality assurance aspects. Team made sure to highlight the tools they utilize for this activity and ultimately, team tested the developed product (initially developed application) against the initial set of test cases. Record keeping for the test case results was of the essence as the team kept on progressing with the design.<br><br>**Entrance Criteria**: Features of the design document and the use-case model.<br><br>**Exit Criteria**: Overall testing, bug tracking and proper use-case execution.<br><br>**ACTIVITY [Discovering Non-Functional Requirements]:** As part of this activity, team identified non-functional/extra requirements that the team believed were important but do not fall into any other documentation category. These were included as an additional Extra Requirement document as part of the deliverables.<br><br>**Entrance Criteria**: Features of the design document, test plan and the use-case model.<br><br>**Exit Criteria**: Creation of any non-functional/extra requirements documentation.<br><br>**ACTIVITY [Upgrade Use-Case Model and Project Plan]:** Main purpose of this activity was be to update the initial use-case model and project plan in order to better highlight the direction in which the software development process will be moving as the project matures.<br><br>**Entrance Criteria**: Input: Initial Use-Case document and the Project Plan document.<br><br>**Exit Criteria**: Output: Enhanced Use-Case document and the Project Plan document as required.|
|**Construction Stage**| **ACTIVITY [Scramble Game v1.0: Initial Coding]:** The purpose of this activity was be to writing code for the initial version of the application based on what was there in the design and the use-case document. Team utilized the use cases from the use case document and the front end GUI prototypes from the design document in order to realize the interface development tasks. On the other hand, class diagram/deployment diagram from the design document was used to implement the back end functionality of the application. Although, main focus of the team was to completely implement what is there in the use-case document, however, there were certain aspects/features of the application that required continuous improvement over the duration of the project.<br><br>**Entrance Criteria**: Input: Use-Case document, Project Plan document or any other non-functional requirements.<br><br>**Exit Criteria**: Version v1.0 of the application was made available with intention to realize all use-cases.<br><br>**ACTIVITY [Testing v1.0]:** Next major step after the initial version of the application was available was to execute the initial set of test cases. This activity used the test case document and highlighted areas of the code/application which may require improvement.<br><br>**Entrance Criteria**: Utilizing the test cases in the Test Plan document and v1.0 of the scramble application<br><br>**Exit Criteria**: Acquiring test results after all the tests cases are executed and updating the test cases if required.<br><br>**ACTIVITY [User Manual v1.0]:** With the initial/beta version of the application ready to be used at this stage, the purpose of this activity was to create a standard document highlighting the user related features and working of the application that would be of interest to the end user/customer.<br><br>**Entrance Criteria**: Inputs from the initial version of the application, use cases, design document, non-functional requirements and feed back via the test cases.<br><br>**Exit Criteria**: Generation of a detailed user manual v1.0 explaining to a customer that how the application works along with its various capabilities.|
|**Transition Stage**| **ACTIVITY [Scramble Game Final Version]:** This activity was crucial as whatever feedback the team received up until this point regarding general user experience and the results from the execution of the test cases was now being put through final phase in order to generate the final version of the scramble application. <br><br>**Entrance Criteria**: Input was the v1.0 of the application along with suggested improvements from the within the team.<br><br>**Exit Criteria**: Output is the enhanced version of the application (Final Version).<br><br>**ACTIVITY [Testing v2.0]:** Similar to the activities in the elaboration stage, final set of test cases were executed on the final version of the application to verify its proper functionality. The intention of the team was to pass all the test cases by the end of this activity and also to make sure that the application is in accordance with all the design document features and the use cases.<br><br>**Entrance Criteria**: For comparison, both v1.0 and Final versions of the application were used along with the final set of test cases.<br><br>**Exit Criteria**: Application able to pass all the test cases in the final Test Plan document.<br><br>**ACTIVITY [Final Revision of the Documents]:** As the final activity of the project, it was essential to update all of the requirement documents. This was similar to the final activities of the elaboration and the construction stages where use case and design documents were updated and user manual was created. As documentation is an iterative process, once the final version of the application was available, if required the UseCaseModel, DesignDocument, TestPlan and UserManual would reflect that.<br><br>**Entrance Criteria**: Input is the final version of the application along with all the above mentioned documents<br><br>**Exit Criteria**: Finalized versions of all the documents accurately reflecting what is implemented.|


## 3 Team

<!--*Describe the team and their roles (there may be more roles than there are team members)*-->

<!--- *Team members' names*
- *Roles, with a short description of each role*
- *Table showing which team member(s) has which role(s)*-->

### Team Members

| Name | GT email ID |
| :-----: | :----------------- |
| Isaac Silva | ```isilva6@gatech.edu``` |
| Mukul Pai | ```mpai8@gatech.edu``` |
| Saad Khan | ```skhan315@gatech.edu``` |

### Development Team Role Description

**Software Architect**

This team member will make high-level design choices and dictate technical standards, including software coding standards, tools, and platforms. The team member will make high-level design choices much more often than low-level choices. Software architect may also be engaged in the design of the architecture of the application environment, or may focus entirely on the design methodology of the code.

**Software Developer**

Tasks of the Software Developer will be to utilize debugging and problem-solving approach in order for developing elemental data structures and working to realize all the use case and design considerations. This team member will contribute to continuously improve software development strategies and would also coordinate any communication pertaining to the external web service (EWS).

**Product Owner**

This member will be main user of the application and will have solid understanding of the requirements and expectations from the project, understanding of users, the market place, the competition and trends for the domain or type of system being developed. This member might also assist the software architect and software developer to make sure that these user interaction elements are synchronized with all their corresponding classes/methods.

**Project Manager**

Team member in this role will be responsible for maintaining the comprehensive architecture and make sure that the application design attains requirements. For documentation purposes, this team member will be responsible for taking information from rest of the team in order to generate/maintain all the documentation/deliverables pertaining to the project. Person in this role will also keep a track of all the design/choices team takes as the project progress through its various stages.

**Software Tester**

Primarily, team member in this role will be responsible for all aspects of application testing such as unit, integration, etc. As the application development process progresses, software tester will keep a record of all the required test cases and will make sure that subsequent versions of the application are producing the desired results. In the case when a particular test does not pass, the software tester will inform and follow-up with the software developer in order to get that issue resolved.


### Development Team Role Assignments

| Name | Assignment |
| :-----: | :----------------- |
| Isaac Silva | Software Architect, Software Tester|
| Mukul Pai | Product Owner, Software Developer|
| Saad Khan | Project Manager, Software Tester|


