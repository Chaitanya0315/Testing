
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
|    v1.0     |    10/06/2017                 |   Team 47                       |           *First draft*                 |
|    v2.0     |    10/13/2017                 |   Team 47                       |           *Few test cases from the Test Plan were tried and status was updated in this document. An additional test was also added to this document.*                 |

## 1 Testing Strategy

### 1.1 Overall strategy

<!--*This section should provide details about your unit-, integration-, system-, and regression-testing strategies. In particular, it should discuss which activities you will perform as part of your testing process, and who will perform such activities.*-->

Overall strategy for testing the application is to acquire fair perspective on how individual components of the application perform. Sequence of tests will be conducted in order to make sure that each component of the application is performing properly. This is an extremely important part of the software development process and will help the team determine areas of the code which require more attention so that the software development process proceeds fluently and effortlessly.

Tests created by the team will first make sure that all the different components of the application will run smoothly in individual capacity without any hindrance. After it is ensured that individual  components are correctly working independently, integration testing will be deployed to verify interaction between components. As an example, a typical unit test for the Login GUI will check proper working of GUI in its entirety, checking for proper information flow, edge cases/boundary conditions, error messages/exceptions, etc. For the case where integration testing will be used, for example: a test may be carried out to check proper working of Login GUI and Player Profile GUI by making sure that both modules will provide desired inputs/outputs to each other while the application is running.

As the programming part of the application streamlines and the product matures, regression testing will also be conducted. As regression testing helps compare valid code between new and previous software builds, it will be carried out for each build of the software application and results will be compared with expected results in order to catch software bugs. Final piece of the picture will be system testing, which will help the team evaluate complete performance of the final software product. System testing will include scenarios such as testing limits of the application by maximizing number of unsolved scrambles or testing the time required to create a scramble, refresh to view an alternate scramble, switching between activities, etc.

The process of creating test scenarios will be a team effort as each member will have a different intuition as to how a particular piece in the application is performing.

### 1.2 Test Selection

<!--*Here you should discuss how you are going to select your test cases, that is, which black-box and/or white-box techniques you will use. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*-->

Primarily, test cases will be extracted from the use cases and junit/esspresso tests will be utilized in order to make sure that chunks of code are generating the desired output. The tests will be selected in a way that they cover wide spectrum of component functionality. This way, if an error is identified, team will be able to focus on that particular error and precise chunk of code causing this error to occur. At the time of creation, this document includes all the possible tests, the team could think of. As the application implementation process progresses, team might add/modify these tests.

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
|1.|Create New Player successfully|User enters first name, last name, desired username, email id|Verified unique user id is generated with appropriate Success message is shown to the user|Verified unique user id is generated with appropriate Success message is shown to the user|Pass|To test that the application generates a unique user id and creates a player correctly|
|2.|Create New Player unsuccessfully|User enters first name, last name, desired username, invalid email id|New player creation is rejected with an error message "Invalid Email"||No Covered|To test that the application fails to create a new player if the email id is invalid|
|3.|Create New Player unsuccessfully|User enters first name, last name, desired username, already existing email id|New player creation is rejected with an error message "Already Exists"||Not Covered|To test that the application fails to create a new player if the email id already exists in the system|
|4.|Player Logins successfully|User enters a unique username|Verified user successfully logs into the application|Verified user successfully logs into the application|Pass|To test that an existing player is able to login into application successfully|
|5.|Player Logins unsuccessfully|User enters a username that has no player profile in the system|User is rejected with an error message "Invalid Username"|User is rejected with an error message "Invalid Username"|Pass|To test that a user is unable to login into application successfully if the username does nto exist in the system|
|6.|Player creates a new word scramble successfully|Player enters an unscrambled phrase and its clue|A new word scramble is created once the user is satisfied with a resulting success message|A new word scramble is created once the user is satisfied with a resulting success message|Pass|To test that a new word scramble is created with a unique  ID and  appropriate success alert message is displayed|
|7.|Player creates a new word scramble successfully and then is unable to edit it once unique ID is assigned|Player enters an unscrambled phrase and its clue and clicks the submit button| Application goes to the unsolved scramble list immediately after OK is clicked on the resulting success message after scramble creation|Application goes to the unsolved scramble list immediately after OK is clicked on the resulting success message after scramble creation|Pass|To test that application does not allow the user to modify a scramble once it is created with a unique ID|
|8.|Player is able to scramble the phrase successfully|Player enters an unscrambled phrase and its clue and reptitively clicks the scramble button|A new word scramble is generated at each click|A new word scramble is generated at each click|Pass|To test that a new word scramble is created each time the user clicks the cramble button|
|9.|Player solves a word scramble successfully|Player enters a solution phrase and clicks the submit button|Application verifies the word scramble solution and displays a success message|Application verifies the word scramble solution and displays a success message|Pass|To test that an appropriate success alert/message is displayed with the unique scramble ID and no. of attempts when that scramble is solved|
|10.|Player solves a word scramble unsuccessfully|Player enters a solution phrase and clicks the submit button|Application verifies the word scramble solution and displays a failure message|Application verifies the word scramble solution and displays a failure message|Pass|To test that an appropriate failure alert/message is displayed with the unique scramble ID and no. of attempts when that scramble remains unsolved|
|11.|Player saves an in-progress word scramble  successfully|Player enters a solution to a word scramble and clicks the save button|Application verifies the word scramble save button is clicks and displays a game saved message|Application verifies the word scramble save button is clicks and displays a game saved message|Pass|To test that an appropriate in-progress saved game alert/message is displayed with the unique scramble ID and no. of attempts up until that point|
|12.|Player is able to view list of unsolved word scrambles successfully|Player clicks 'Solve Word Scramble' button from the player profile menu|Unsolved word scrambles are successfully displayed by unique ID and ordered by in-progress games and the no. of attempts shown first||Not Covered|To test unsolved word scrambles activity is successfully displayed|
|13.|Player resumes an in-progress word scramble|Player selects an in-progress scrmable from unsolved Scramble list|Verify that the in-progress scramble is retrieved with the previously stored state ||Not Covered|To test that an existing word scramble is restored with the previously stored state|
|14.|Player exits a word scramble|Player selects to exit the game by clicking the 'Back to Scramble List' option from scramble game page|Verify that the in-progress scramble state is preserved and player is directed to unsolved game list||Not Covered|To test that the last state of the word scramble is preserved and the Player is directed to to unsolved game list|
|15.|Player is able to view player statistics|Player clicks 'Player Statistics' option from Players profile page|Verify that the Player statistics page is loaded with below information sorted by csrambles solved:- a. First name, last name, b. Word scramble solved, c. Word scramble created, d. Scramble created vs Solved by others ratio||Not Covered|To test that a player is able to retrieve and view player statistics|
|16.|Player is able to view scramble statistics|Player clicks 'Scramble Statistics' option from Players profile page|Verify that the Scramble  statistics page is loaded with below information sorted by number of time a scramble was solved:- a. unique game ID, b. number of time a scramble was solved, c. category of that player as either the creator of the game or solver of the game||Not Covered|To test that a player is able to retrieve and view word scramble statistics|
|17.|Player logs out|Player logs out of account|Player is able to exit the game||Not Covered|To test that a player successfully exits the game|
|18.|Player goes back to the Login page|Player clicks the 'Back to Login Page' to move from palyer profile activity back to the login activity|Player is able to go back to the login page||Not Covered|To test that a player can successfully go to the login page from the player profile page|
|19.|Player goes back to the player profile page|Player clicks the 'Back to Player Profile' to move from scramble statistics activity, player statistics activity, create word scramble activity or solve the scramble activity back to the player profile activity|Player is able to go back to the player profile||Not Covered|To test that a player can successfully go to the player profile page from scramble statistics activity, player statistics activity, create word scramble activity or solve the scramble activity|
|20.|Player is unable to connect due to lack of internet/WiFi connectivity|Player clicks any button to move around the application|Player is unable to connect and use any functionality in the application|||To test that a player unsuccessful to move navigate around the application due to lack of internet/WiFi connectivity|
