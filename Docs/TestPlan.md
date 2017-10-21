
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
| :-----: | :-----------------: | :----------------------: | :------------------------ |
|    v1.0     |    10/06/2017                 |   Team 47                       |           *First draft*                 |
|    v1.1     |    10/13/2017                 |   Team 47                       |           *Few test cases from the Test Plan were tried and status was updated in this document. An additional test was also added to this document.*                 |
|    v1.2     |    10/20/2017                 |   Team 47                       |           *Final test plan*                 |

## 1 Testing Strategy

### 1.1 Overall strategy

<!--*This section should provide details about your unit-, integration-, system-, and regression-testing strategies. In particular, it should discuss which activities you will perform as part of your testing process, and who will perform such activities.*-->

Overall strategy for testing the application is to acquire fair perspective on how individual components of the application perform. Sequence of tests will be conducted in order to make sure that each component of the application is performing properly. This is an extremely important part of the software development process and will help the team determine areas of the code which require more attention so that the software development process proceeds fluently and effortlessly.

Tests created by the team will first make sure that all the different components of the application will run smoothly in individual capacity without any hindrance. After it is ensured that individual  components are correctly working independently, integration testing will be deployed to verify interaction between components. As an example, a typical unit test for the Login GUI will check proper working of GUI in its entirety, checking for proper information flow, edge cases/boundary conditions, error messages/exceptions, etc. For the case where integration testing will be used, for example: a test may be carried out to check proper working of Login GUI and Player Profile GUI by making sure that both modules will provide desired inputs/outputs to each other while the application is running.

As the programming part of the application streamlines and the product matures, regression testing will also be conducted. As regression testing helps compare valid code between new and previous software builds, it will be carried out for each build of the software application and results will be compared with expected results in order to catch software bugs. Final piece of the picture will be system testing, which will help the team evaluate complete performance of the final software product. System testing will include scenarios such as testing limits of the application by maximizing number of unsolved scrambles or testing the time required to create a scramble, refresh to view an alternate scramble, switching between activities, etc.

The process of creating test scenarios will be a team effort as each member will have a different intuition as to how a particular piece in the application is performing.

### 1.2 Test Selection

<!--*Here you should discuss how you are going to select your test cases, that is, which black-box and/or white-box techniques you will use. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*-->

Primarily, test cases will be extracted from the use cases in order to make sure that chunks of code are generating the desired output. The tests will be selected in a way that they cover wide spectrum of component functionality. This way, if an error is identified, team will be able to focus on that particular error and precise chunk of code causing this error to occur. At the time of creation, this document includes all the possible tests, the team could think of. As the application implementation process progresses, team might add/modify these tests.

### 1.3 Adequacy Criterion

<!--*Define how you are going to assess the quality of your test cases. Typically, this involves some form of functional or structural coverage. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*-->

To check if the test cases created by the team are adequate, the team will try to make sure that these test cases address major chunk of all the functionality of the code, i.e. at least 80% functionality. Checking adequacy this way will help the team have a better understanding of the code and also help minimize most of the errors. This will also help the team to determine if the application is being developed in the correct manner (testing for verification) and also that is the application being developed is correct or not (testing for validation).


### 1.4 Bug Tracking

<!--*Describe how bugs and enhancement requests will be tracked.*-->

In order to track bugs, the application software developer found it more convenient to utilize the capabilities of the Android Studio internal debugger, so the team decided to stick with this approach. Android Studio internal debugger provided quick and easy way to test the application for bugs while the application was being run via the emulator. This way the team was able to resolve the bugs in the code in a quick fashion rather than relying on an external bug-tracking system.

### 1.5 Technology

<!--*Describe any testing technology you intend to use or build (e.g., JUnit, Selenium).*-->

Testing technologies that the team intended to use while developing the word scramble application were JUnit and Espresso, however, most of the testing performed was manual with all team members taking turns in rigorously testing all the different aspects of the final application. With all the eleventh hour changes being made to make the application work, the team felt it was more appropriate to test different features of the application manually. This is in accordance with the requirements for deliverable 4 and each test case description clearly mentions on how to reproduce it and adequately cover all the different functionalities of the application.


## 2 Test Cases

<!--*This section should be the core of this document. You should provide a table of test cases, one per row. For each test case, the table should provide its purpose, the steps necessary to perform the test, the expected result, the actual result (to be filled later), pass/fail information (to be filled later), and any additional information you think is relevant.*-->

| **Test Case ID** | **Purpose** | **Steps** | **Expected Result** | **Actual Result** | **Pass/Fail** |   **Description** |
| --- | --- | --- | --- | --- | --- | --- |
|1|Create New Player successfully|User enters first name, last name, desired username, email id inside the Create New Player UI|Verified unique user id is generated and an appropriate success message is shown to the user with 2 digits appended to avoid duplication|Verified unique user id is generated and an appropriate success message is shown to the user with 2 digits appended to avoid duplication|Pass|To test that the application generates a unique user id and creates a player correctly|
|2|Create New Player unsuccessfully|User enters first name, last name, desired username, invalid email id inside the Create New Player UI|New player creation is rejected with an error message "Enter valid Email ID"|New player creation is rejected with an error message "Enter valid Email ID"|Pass|To test that the application fails to create a new player if the email id is invalid|
|3|Create New Player unsuccessfully|User enters first name, last name, desired username, already existing email id|New player creation is rejected with an message saying "Email id is already registered. Please login with your Player ID or choose another email id."|New player creation is rejected with an message saying "Email id is already registered. Please login with your Player ID or choose another email id."|Pass|To test that the application fails to create a new player if the email id already exists in the system|
|4|Player Logins successfully|User enters a unique username|Verified user successfully logs into the application|Verified user successfully logs into the application|Pass|To test that an existing player is able to login into application successfully|
|5|Player Logins unsuccessfully|User enters a username that has no player profile in the system|User is rejected with an error message "Invalid Username"|User is rejected with an error message "Invalid Username"|Pass|To test that a user is unable to login into the application successfully if the username does not exist in the system|
|6|Player creates a new scramble successfully|Player enters an unscrambled phrase and its clue according to the requirements|Once the user is satisfied, a new scramble is created with a resulting success message|Once the user is satisfied, a new scramble is created with a resulting success message|Pass|To test that a new scramble is created with a unique  ID and  appropriate success alert message is displayed|
|7|Player creates a new word scramble successfully and then is unable to edit it once unique ID is assigned|Player enters an unscrambled phrase and its clue and clicks the submit button| Application goes to the unsolved scramble list immediately after OK is clicked on the resulting success message after scramble creation not allowing the player to edit the scramble he/she just created| Application goes to the unsolved scramble list immediately after OK is clicked on the resulting success message after scramble creation not allowing the player to edit the scramble he/she just created|Pass|To test that application does not allow the user to modify a scramble once it is created with a unique ID|
|8|Player is able to repeatedly scramble the phrase successfully while creating it|Player enters an unscrambled phrase and its clue and reptitively clicks the 'Scramble!!!' button|A new scramble is generated at each time the 'Scramble!!!' button is clicked|A new scramble is generated at each time the 'Scramble!!!' button is clicked|Pass|To test that a new scramble is created each time the user clicks the'Scramble!!!' button|
|9|Player is unable to create a scramble if no clue is provided|Player enters an unscrambled phrase and does not enter any clue|User is unable to 'Accept' a scramble and gets an error message   Please provide a clue for the unscrambled phrase"|User is unable to 'Accept' a scramble and gets an error message   Please provide a clue for the unscrambled phrase"|Pass|To test that the new scramble is not created if user does not provide any clue|
|10|Player solves a scramble successfully|Player enters a solution phrase and clicks the submit button|Application verifies the scramble solution and displays a success message 'Congratulations'|Application verifies the scramble solution and displays a success message 'Congratulations'|Pass|To test that an appropriate success alert/message is displayed with the unique scramble ID and no. of attempts when that scramble is solved|
|11|Player solves a scramble unsuccessfully|Player enters a solution phrase and clicks the submit button|Application verifies the scramble solution and displays a failure message|Application verifies the scramble solution and displays a failure message|Pass|To test that an appropriate failure alert/message is displayed with the unique scramble ID and no. of attempts when that scramble remains unsolved|
|12|Player saves an in-progress scramble  successfully|Player enters a solution to a scramble and clicks the save button|Application verifies the scramble save button is clicked and displays a game saved message and moves back to the scramble list|Application verifies the scramble save button is clicked and displays a game saved message and moves back to the scramble list|Pass|To test that an appropriate in-progress saved game alert/message is displayed with the unique scramble ID and no. of attempts up until that point|
|13|Player is able to view list of unsolved scrambles successfully|Player clicks 'Solve Scramble' button from the player home page|Unsolved scrambles are successfully displayed by unique ID and ordered so that in-progress games are shown first|Unsolved scrambles are successfully displayed by unique ID and ordered so that in-progress games are shown first|Pass|To test unsolved scrambles activity is successfully displayed|
|14|Player successfully resumes an in-progress scramble|Player selects an in-progress scramble from unsolved Scramble list|Verify that the in-progress scramble is retrieved in the previously stored state with the 'Enter your solution' text box containing the last saved probable solution|Verify that the in-progress scramble is retrieved in the previously stored state with the 'Enter your solution' text box containing the last saved probable solution|Pass|To test that an existing scramble is restored with the previously stored state|
|15|Player exits a word scramble successfully|Player selects to exit the game at any time by clicking the 'BACK TO SCRAMBLE LIST' option from scramble game page|The player is directed to unsolved scramble list leaving the srcamble in the initial state|The player is directed to unsolved scramble list leaving the srcamble in the initial state|Pass|To test that the scramble is taken to its initial state and the Player is directed to to unsolved scramble list|
|16|Player is able to view player statistics successfully|Player clicks 'Player Statistics' option from player's home page|Verify that the Player statistics page is loaded with below information sorted by scrambles solved:- a. First name, last name, b. Scrambles solved, c. Scramble created, d. Solved by others vs Scramble created ratio |Verify that the Player statistics page is loaded with below information sorted by scrambles solved:- a. First name, last name, b. Scrambles solved, c. Scramble created, d. Solved by others vs Scramble created ratio |Pass|To test that a player is able to retrieve and view player statistics|
|17|Player is able to view scramble statistics successfully|Player clicks 'Scramble Statistics' option from player's home page|Verify that the Scramble  statistics page is loaded with below information sorted by number of time a scramble was solved:- a. unique scramble ID, b. number of time a scramble was solved, c. category of that player as either the creator of the game or solver of the game|Verify that the Scramble  statistics page is loaded with below information sorted by number of time a scramble was solved:- a. unique scramble ID, b. number of time a scramble was solved, c. category of that player as either the creator of the game or solver of the game|Pass|To test that a player is able to retrieve and view scramble statistics|
|18|Player logs out successfully|Player logs out of account by clicking the 'LOGOUT' button on the player's home page|Player is able to exit the game and go back to the 'WELCOME TO SCRAMBLE APP!' login page|Player is able to exit the game and go back to the 'WELCOME TO SCRAMBLE APP!' login page|Pass|To test that a player successfully exits their account|
|19|Player goes back to the player profile page successfully|Player clicks the 'Back to Player Profile' to move from scramble statistics activity, player statistics activity, create scramble activity or solvea scramble activity back to the player home page activity|Player is able to go back to the player profile successfully|Player is able to go back to the player profile successfully|Pass|To test that a player can successfully go to the player profile page from scramble statistics activity, player statistics activity, create scramble activity or solve the scramble activity|
|20|Player is unable to connect due to lack of internet/WiFi connectivity|Player clicks any button to move around the application|Player is unable to connect and use any functionality in the application|Player is unable to connect and use any functionality in the application|Pass|To test that a player unsuccessful to move navigate around the application due to lack of internet/WiFi connectivity|

