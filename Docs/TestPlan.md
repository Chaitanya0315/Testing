
# Test Plan

<!--*This is the template for your test plan. The parts in italics are concise explanations of what should go in the corresponding sections and should not appear in the final document.*-->

**Author**:  Team 47 

| Name | GT email ID |
| :-----: | :----------------- |
| Isaac Silva | ```isilva6@gatech.edu``` |
| Mukul Pai | ```mpai8@gatech.edu``` |
| Saad Khan | ```skhan315@gatech.edu``` |

**Document Tracking**: Following chart is used to log all the changes made to this document.

| Version | Date of edit/change | Who made the edit/change | Description of edit/change |
| :-----: | :-----------------: | :----------------------: | :------------------------: |
|    v1.0     |    10/04/2017                 |   Team 47                       |           *first draft*                 |

## 1 Testing Strategy

### 1.1 Overall strategy

<!--*This section should provide details about your unit-, integration-, system-, and regression-testing strategies. In particular, it should discuss which activities you will perform as part of your testing process, and who will perform such activities.*-->

Overall strategy for testing the application is to acquire fair perspective on how individual components of the application perform. Sequence of tests will be conducted in order to make sure that each component of the application is performing properly. This is an extremely important part of the software development process and will help the team determine areas of the code which require more attention so that the software development process proceeds fluently and effortlessly.

Tests created by the team will first make sure that all the different components of the application will run smoothly in individual capacity without any hindrance. After it is ensured that individual  components are correctly working independently, integration testing will be deployed to verify interaction between components. As an example, a typical unit test for the Login GUI will check proper working of GUI in its entirety, checking for proper information flow, edge cases/boundary conditions, error messages/exceptions, etc. For the case where integration testing will be used, for example: a test may be carried out to check proper working of Login GUI and Player Profile GUI by making sure that both modules will provide desired inputs/outputs to each other while the application is running.

As the programming part of the application streamlines and the product matures, regression testing will also be conducted. As regression testing helps compare valid code between new and previous software builds, it will be carried out for each build of the software application and results will be compared with expected results in order to catch software bugs. Final piece of the picture will be system testing, which will help the team evaluate complete performance of the final software product. System testing will include scenarios such as testing limits of the application by maximizing number of unsolved scrambles or testing the time required to create a scramble, refresh to view an alternate scramble, switching between activities, etc.

The process of creating test scenarios will be a team effort as each member will have a different intuition as to how a particular piece in the application is performing.

### 1.2 Test Selection

<!--*Here you should discuss how you are going to select your test cases, that is, which black-box and/or white-box techniques you will use. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*-->

Primarily, test cases will be extracted from the use cases and junit/esspresso tests will be utilized in order to make sure that chunks of code are generating the desired output. The tests will be selected in a way that they cover wide spectrum of component functionality. This way, if an error is identified, team will be able to focus on that particular error and precise chunk of code causing this error to occur.

### 1.3 Adequacy Criterion

<!--*Define how you are going to assess the quality of your test cases. Typically, this involves some form of functional or structural coverage. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*-->

To check if the test cases created by the team are adequate, the team will try to make sure that these test cases address major chunk of all the functionality of the code, i.e. at least 80% functionality. Checking adequacy this way will help the team have a better understanding of the code and also help minimize most of the errors. This will also help the team to determine if the application is being developed in the correct manner (testing for verification) and also that is the application being developed is correct or not (testing for validation).


### 1.4 Bug Tracking

<!--*Describe how bugs and enhancement requests will be tracked.*-->

In order to track bugs, code changes and progress during the development phase, team has decided to use Bugzilla. It is an open-source, effective "Bug-Tracking System" that will allow the team to keep track of outstanding bugs pertaining to the word scramble application. Team has chosen Bugzilla due to its ease of usage, however, if the team feels that another bug tracking tool is more appropriate, team will switch to that tool and this document will be updated subsequently.

### 1.5 Technology

<!--*Describe any testing technology you intend to use or build (e.g., JUnit, Selenium).*-->

Testing technologies that the team intends to use while developing the word scramble application are JUnit and Espresso. Team feels more accustomed with the testing frame work of JUnit and also the fact that it is precisely designed to be used with Java is an added factor. For automated UI tests the Espresso UI test framework will utilized in Android Studio. However, during the development process if the team feels that another testing tool is more appropriate, team will switch on to that technology and this document will be updated accordingly.  

## 2 Test Cases

<!--*This section should be the core of this document. You should provide a table of test cases, one per row. For each test case, the table should provide its purpose, the steps necessary to perform the test, the expected result, the actual result (to be filled later), pass/fail information (to be filled later), and any additional information you think is relevant.*-->

| **Test Case ID** | **Purpose** | **Steps** | **Expected Result** | **Actual Result** | **Pass/Fail** |   **Description** |
| --- | --- | --- | --- | --- | --- | --- |
| 1. | Create New Player | Enter user Fname & Lname, desired Username, emailid | Verify unique user id is generated with appropriate Success message | | | Test the application generates unique user id |
| 2. | Player Login | Enter unique user id | Verify successful login into application | | | Test a player is able to login into application successfully |
| 3. | Create new Scramble | Enter unscrambled phrase and clue | Verify new word scramble is created | | | Test a new word scramble is created with a unique scramble ID and appropriate success alert message is displayed |
| 4. | Solve Word scramble | Enter the solution to a word scramble and submit | Verify Word Scramble solved alert is received | | | Test appropriate alert is displayed with the scramble ID when a Word Scramble is solved |
| 5. | Save in-progress Word Scramble | Enter the solution to a word scramble and save | Verify Word Scramble saved alert is received | | | Test appropriate alert is displayed with the scramble ID when a Word Scramble is saved |
| 6. | View list of unsolved Word Scrambles | Select 'View Unsolved Scrambles' from Players Home page | Verify unique user id is generated with appropriate Success messageVerify Unsolved Word scrambles are successfully displayed by identifier id and ordered by in-progress games shown first | | | Test Unsolved Word scrambles are successfully displayed |
| 7. | Resume Word Scramble | Select an In-progress Scramble from Unsolved Scramble list | Verify the In-progress scramble is retrieved with the previously stored state | | | Test an existing word scramble is restored with the previously stored state |
| 8. | Exit Word Scramble | Select Exit game option from Scramble game page | Verify the In-progress scramble state is preserved and player is directed to home page | | | Test the last state of the Word scramble is preserved and the Player is directed to his home page |
| 9. | Retrieve and View Player Statistics | Select 'View Statistics' option from Players Home page | Verify Player statistics page is loaded with below information-a. Word scramble solved, b. Word scramble created, c. Scramble created vs Solved by others ratio | | | Test a player is able to retrieve and view his statistics |
| 10. | View list of unsolved Word Scrambles | Select 'View Unsolved Scrambles' from Players Home page | Verify Unsolved Word scrambles are succesffuly displayed by identifier id and ordered by in-progress games shown first | | | Test Unsolved Word scrambles are succesfully displayed  |
