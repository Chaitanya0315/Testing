
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

Overall strategy for testing the application is to acquire fair perspective on how indivual components of the application perform. Sequence of tests will be conducted in order to make sure that the each component of the application is performing properly. This is an extremely important part of the software development process and will help the team determine areas in the process which require more attention so that the software development process proceeds fluently and effortlessly.

Tests created by the team will first make sure that all the different components of the application will run smoothly in individual capacity without any hinderence. After it is ensured that indiviudal components are correctly working independently, integration testing will be deployed to verify interaction between components. As an example, a typical unit test for the Login GUI will check proper working of GUI in its entirety, checking for proper information flow, edge cases/boundary conditions, error messages/exceptions, etc. For the case where integration testing will be used, a test may be carried out to check proper working of Login GUI and Player Profile GUI by makign sure that both modules will provide desired inputs/outputs to each other while the application is running.

As the programming part of the application streamlines and the product matures, regression testing will also be conducted. As regression testing helps compare valid code between new and previous software builds, it will be caried out for each build of the software application and results will be compared with expected results in order to catch software bugs. Final piece of the picture will be system testing, which wil help the team evaluate complete performance of the final software product. System testing will include sceanrios such as testing limits of the application by maximizing number of unsolved scrambles or testing the time required to create a scramble, refresh to view an alternate scramble, switching between activities, etc.

The process of creating test scenarios will be a team effort as each member will have a different intuition as to how a particular piece in the application is performing.

### 1.2 Test Selection

*Here you should discuss how you are going to select your test cases, that is, which black-box and/or white-box techniques you will use. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*

Primarily, test cases will be extracted from the use cases and junit/esspresso tests will be utilized in order to make sure that chunks of code are generating the desired output. The test will be selected in a way that they cover wide spectrum of component functionality. This way, if an error is identified, team will be able to focus on that particular error and precise chunk of code causing this error to occur.

### 1.3 Adequacy Criterion

*Define how you are going to assess the quality of your test cases. Typically, this involves some form of functional or structural coverage. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*

### 1.4 Bug Tracking

*Describe how bugs and enhancement requests will be tracked.*

### 1.5 Technology

*Describe any testing technology you intend to use or build (e.g., JUnit, Selenium).*

## 2 Test Cases

*This section should be the core of this document. You should provide a table of test cases, one per row. For each test case, the table should provide its purpose, the steps necessary to perform the test, the expected result, the actual result (to be filled later), pass/fail information (to be filled later), and any additional information you think is relevant.*
