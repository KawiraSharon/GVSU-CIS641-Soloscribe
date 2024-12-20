# Overview
BankingMadeSimple is a web-based application that primarily focuses on ensuring simple and secure money transactions, particularly money transfers. The application implements simple Sign Up, Sign In, Sign Out, Displays Balance of User Account, Send Money, Transaction Overview, and All Transactions features, all interweaved to create a simple, intuitive User Interface that aims at enhancing user satisfaction, minimizing technical issues encountered, and eventually achieving user retention.

# Software Requirements
This section contains a description of the functional and non-functional requirements of the application. The functional requirements focus on feature behavior and what the system does for the user, while the non-functional requirements focus on the scalability, performance, security, reliability, and usability of the system.

## Functional Requirements

### **Sign Up**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR1 | The system shall provide a sign-up hyperlink on the sign-in page that redirects users to a 'Sign Up' page where they can enter their details to create an account. |
| FR2 | The system shall provide a registration form with personal details and a 'Sign Up' button to allow new users to create an account and register on the platform.. |
| FR3 | The system shall ensure that the email provided during sign-up is unique to allow for successful account creation. |
| FR4 | The system shall prevent users from creating accounts with an email that is already registered. |
| FR5 | The system shall redirect users to the dashboard page after they successfully complete the sign-up process and click the 'Sign Up' button. |

---

### **Sign In**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR6 | The system shall provide users with email and password fields to authenticate and sign them into the platform. |
| FR7 | The system shall allow registered users to sign in by entering their email and password, and clicking the 'Sign In' button. |
| FR8 | The system shall not allow any unregistered users successful login attempts. |
| FR9 | The system shall autosave sign-in details on devices where verified users have previously logged in. |
| FR10 | The system shall allow verified users to bypass sign-in process on devices they had previously signed in. |
| FR11 | The system shall keep users signed in on previously logged-in devices until they manually sign out or change their password. |

---

### **Sign Out**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR12 | The system shall display a sign-out icon on the bottom-left sidebar that active users can use to end their session. |
| FR13 | The system shall allow active platform users to sign out by clicking the sign-out icon. |
| FR14 | The system shall redirect users to the sign-in page upon successful sign-out. |
| FR15 | The system shall automatically sign out all active sessions when a user changes their password. |
| FR16 | The system shall ensure that the user session ends when the sign-out icon is clicked. |

---

### **Send Money**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR17 | The system shall allow users to send money to other registered users on the platform. |
| FR18 | The system shall verify the recipient’s email address before processing the transaction. |
| FR19 | The system shall allow users to cancel the transaction during processing if they choose not to finalize it. |
| FR20 | The system shall allow users to enter any amount they wish to send, provided it includes a comma or period as a separator. |
| FR21 | The system shall display an "Amount is too short" message for incorrectly formatted amounts. |

---

### **All Transactions**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR22 | The system shall display detailed information for each transaction such as amount spent, and status. |
| FR23 | The system shall allow users to view all past transactions and their accompanying details. |
| FR24 | The system shall display transactions in chronological order, with the most recent transactions appearing first. |
| FR25 | The system shall store transaction history. |
| FR26 | The system shall display current user balance on top of the 'All Transactions' page. |
| FR27 | The system shall refresh the 'All Transactions' page after each new transaction. |

---

### **Total Balance**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| FR28 | The system shall display the user's balance on the top of the dashboard for easy visibility. |
| FR29 | The system shall display the balance in both a larger and emboldened font to further enhance visibility. |
| FR30 | The system shall ensure the balance is visible upon user sign-in, reducing the need for additional clicks to view their balance. |
| FR31 | The system shall update the total balance after each transaction. |
| FR32 | The system shall display the balance with a comma separator, following the expected in-app format to guide users when transacting.. |

---


## Non-Functional Requirements

### **Security**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| NFR1 | The system shall only allow verified and registered users with emails that matches their passwords to sign into the platform. |
| NFR2 | The system shall automatically sign out active user sessions when they change their passwords. |
| NFR3 | The system shall safely encrypt all user data, including their sign in details, when both at rest and in transit. |
| NFR4 | The system shall automatically lock the user account after five consecutive non-successful sign in attempts. |
| NFR5 | The system shall store all security-related activities, including failed login attempts, for auditing purposes. |

---

### **Usability**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| NFR6 | The system shall offer a very simple, user-friendly interface usable by non-technical users to complete tasks. |
| NFR7 | The system shall provide clear and understandable error messages when the user enters an invalid format for required fields. |
| NFR8 | The system shall offer a fully responsive interface across both desktop and mobile devices. |
| NFR9 | The system shall ensure that all functionalities are easy to use and require minimal clicks. |
| NFR10 | The system shall offer a personalized user experience by giving a welcome message with the user's first name on the dashboard. |

---

### **Performance**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| NFR11 | The system shall ensure automatic access to the user dashboard within 2 seconds for 95% of users upon successful sign-in. |
| NFR12 | The system shall automatically process money transfers within 10 seconds. |
| NFR13 | The system shall respond to user click actions within 1 second. |
| NFR14 | The system shall update transaction history within 1 second after users send or receive money. |
| NFR15 | The system shall handle a minimum of 350 transactions per second at peak load times. |

---

### **Reliability**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| NFR16 | The system shall ensure an uptime of 99.9% throughout the year. |
| NFR17 | The system shall be accessible 24/7 during all weekdays. |
| NFR18 | The system shall automatically recover from network outages within 30 seconds. |
| NFR19 | The system shall support reliable transaction processing even during scheduled maintenance. |
| NFR20 | The system shall ensure data security and integrity even when there are unexpected shutdowns. |

---

### **Scalability**

| ID  | Requirement                                                       |
| :--:| :-----------------------------------------------------------------:|
| NFR21 | The system shall support 36,350 simultaneous users without performance degradation.. |
| NFR22 | The system shall allow maintenance to be performed without affecting system availability or scalability. |
| NFR23 | The system shall handle a 33% increase in transaction operations at peak times without latency. |
| NFR24 | The system shall dynamically allocate resources based on real-time demand to ensure scalability without affecting system availability. |
| NFR25 | The system shall use Appwrite to ensure database queries optimize scalability, even under heavy user load. |

---

# Change management plan
This section outlines the change management plan for the BankingMadeSimple application, emphasizing user adoption and implementation. The goal is to ensure that individual users can easily integrate and adopt the application into their daily banking activities, ensuring a simple, seamless and efficient user experience.

#### Training people to use the application
Incorporating a product tour for first time users. 
- This feature will provide a step by step guidance for first time users to ensure they are not overwhelmed by the features of the application. The tour will help users know where to find each functionality where it begins as follows;
- Begin with a welcome message, shows users where to enter their details securely, the sign in, sign up functionalities.
- Explain the dashboard layout by showing the user where to view their total balance.
- Guide users on how to initiate a money transfer, explain that they complete the action by clicking the 'Send Money' button.
- The tour will show users where to find their transaction history.
- An 'exit tour' button to show that the tour is complete. This option shall however remain in the settings icon that will be implemented in the future. 
- The tour will also offer a 'Next' button when each step is seen, or a 'Skip' tour button, altogether offering the liberty to users to skip the tour altogether.

The application shall incorporate a chatbot and a tech support email.
- Users will be encouraged to use the chatbot for common questions, FAQs and troubleshooting purposes, generally for quick help. They will be encouraged to use the tech support email for more complex inquiries. Users will be asked to provide feedback after interacting with the chatbot and email. This will provide insights on how useful these resources will be, and enable address any areas of improvement.
 
Successes will be identified and reinforced by monitoring, analysing and recording the metrics of user activity like money transfers. That information will be shared as part of a success story that will be used to encourage others to adopt and use the application.

Continuous Training and Updates;
- As new users are onboarded and existing users continue to engage with the application, continuous training and updates will play a critical role in ensuring the app’s ongoing success goes hand in hand with user adoption.
- This will be done by taking the following steps;
- Onboarding new users by giving them a product tour as discussed above.
- Ongoing learning for already existing users where they will be given regular notifications and reminders on any new features and updates.
- Both users will be periodically notified of any underused implemented features and why they should explore them.

User feedback will be collected by conducting surveys and anecdotal feedback.
- First time users will be prompted to provide feedback through surveys and feedback forms. 
- Interviews and casual conversations will be used to collect anecdotal feedback in gaining insights on how users feel about the application, and any areas they may want improved.

Consistent compliance audits
- These will ensure the application functionalities align with legal and standard requirements especially the security, data and privacy regulations.
- Embedding a video that explains how to use the in-app functionalities, so they can easily get themselves acquainted with the application and its functionalities. The video will be periodically updated with any new features.
- User feedback will be collected on any areas of resistance by users, and any technical features introduced and used in the revision and implementation of any necessary changes. Work with the sponsor will also be incorporated to address the areas of feedback and offer any additional required training.

#### Ensuring it integrates within their ecosystem / software
Planning and feasibility analysis
- Understand the current system - assess current systems within the customer's ecosystem and identify any compatibility issues that may arise with using the new banking app, also for future risk mitigation.
- Identify any integration requirements - ensure data formats are catered for, APIs and interfaces as well, and ensure security protocols that ensure data security and integrity are catered for.

Calculate and outline the scope, schedule and cost expected from the integration
- Identify how much time the intergration requires, including when it starts.
- Identify resources needed, including technical expertise and support.
- Identify any potential risks and put in place mitigation strategies.

Put together the planning and feasibility analysis, and calculate the scope, schedule and cost to identiy whether the integration is possible, and make any adjustments to accordingly cater for any potential issues moving forward.

Architecture Modelling
- This step ensures designing of the integration architecture to ensure systems communicate and function together without issues.
- Begin with choosing the integration model - Research on and choose either a hub-and-spoke, middleware or point-to-point model, according to the customer's specific needs.
- Designing the communication blueprint - to define how the systems will communicate by ensuring data loss is avoided. Data formats and structures alignment is catered for.
- Create preliminary and physical designs - UML diagrams and any other high level diagramming and representation of the system architecture should be created. Provide details on how data is expected to flow between the systems.

Implementation
- This phase will see the actual connection of the systems.
- This will be completed following these steps;
- System Testing - the BankingMadeSimple application will be put through rigorous testing to ensure all modules interact seamlessly and work well with each other, the data synchronization, functionality testing, and security testing modules will be specifically rigorously tested to ensure no vulnerabilities.
- Pilot Testing - implement a miniature version of the application to ensure any identified issues are addressed before the whole system is rolled out. User feedback is highly valuable in this phase.
- Go-Live - after successful testing and integration of the application, full deployment will be rolled out to ensure the application is available to users.
- Agile Project Management - throughout the entire implementation phase, agile practices will be implemented to ensure that issues are addressed as they arise, and that any evolving customer needs are met.

Maintenance and support
- This phase will ensure continued optimal performnce of the application.
- Routine Diagnostics - these checks will help ensure the integrated system continues to work as required, and no errors occur during data transmission.
- Performance monitoring - this will ensure any latency, API, and transaction processing issues are identified and corrected early.
- Error resolution - this step will see creation of clear channels to report logs, implement hotfixes and updates as needed are put in place
- Continuous updates - this will be crucial in ensuring any occuring bugs are fixed, and new features are implemented as customer needs and business processes change. 
- User Feedback Loop - this step will typically enhance continous improvement of the integration process as well as the application itself.

#### Ensuring any discovered issues are resolved
Identify, analyze and prioritize the issues.
- Thoroughly understand the root cause of the problem, by gathering information on the problem, understanding its symptoms, and determining its effects on users.
Assign the issue to the right person for resolution purposes
- Choose the right member, with the right communication skills, as well as the required expertise and knowledge to resolve the issue.
Implementing a solution fix depending on the gravity of the issue. 
- Code may need to be modified, or configurations adjusted, through development of the solution. Encourage collaboration between members as the bug is being fixed, and test the fix.
Once the issue is resolved, involve stakeholders to ensure their expectations are met.
Document the issue resolution.
- Provide details on what caused the bug, the fix implemented, results of the fix implementation, and feedback, approval from the stakeholders. The documentation will be a valuable tool for future reference and in the continuous improvement of the application.
- Notify relevant parties on closure of the issue.
- Once the issue is resolved, stakeholders, users and any other relevant parties will be notified that it is resolved.
Continous monitoring and preventative measures.
- This step will ensure smooth operations of the system, it will also ensure that in case the issue arises again, it is addressed promptly.


# Traceability Links

### Use Case Diagram 1 Traceability

| Artifact ID | Use Case Name        | Requirement ID        |
|:---------------:|:------------------------:|:----------------------------:|
| UseCase1        | Sign Up                  | FR1, FR2, FR3, FR4, FR5      |
| UseCase2        | Sign In                  | FR6, FR7, FR8, FR9, FR10, FR11 |
| UseCase3        | Sign Out                 | FR12, FR13, FR14, FR15, FR16 |
| UseCase4        | Send Money               | FR17, FR18, FR19, FR20, FR21 |
| UseCase5        | View All Transactions    | FR22, FR23, FR24, FR25, FR26, FR27 |
| UseCase6        | View Total Balance       | FR28, FR29, FR30, FR31, FR32 |

---

### Use Case Diagram 2 Traceability

| Artifact ID | Use Case Name        | Requirement ID        |
|:---------------:|:------------------------:|:----------------------------:|
| UseCase1        | Sign In                  | FR6, FR7                      |
| UseCase2        | Reset Password           | TBD                           |
| UseCase3        | View Total Balance       | FR28              |
| UseCase4        | Sign Out                 | FR12                    |

---

### Use Case Diagram 3 Traceability

| Artifact ID | Use Case Name        | Requirement ID        |
|:---------------:|:------------------------:|:----------------------------:|
| UseCase1        | Update Account Balance   | FR31                   |
| UseCase2        | Withdraw Money           | TBD                    |
| UseCase3        | Transfer Funds/Money     | FR17                   |
| UseCase4        | Deposit Money            | TBD                    |

---

### Activity Diagram 2 Traceability

| Artifact ID | Activity Name       | Requirement ID        |
|:---------------:|:------------------------:|:----------------------------:|
| Activity_Diagram-2 | Sign In                | FR6, FR7                      |
| Activity_Diagram-2 | Reset Password         | TBD                           |
| Activity_Diagram-2 | View Total Balance     | FR28              |

---

### Activity Diagram 3 Traceability

| Artifact ID | Activity Name        | Requirement ID       |
|:---------------:|:------------------------:|:----------------------------:|
| Activity_Diagram-3 | Withdraw Money         | TBD             |
| Activity_Diagram-3 | Transfer Money (Funds) | FR17, NFR7                    |
| Activity_Diagram-3 | Deposit Money          | TBD             |
| Activity_Diagram-3 | Update Account Balance | FR31                   |

---

### **Class Diagram Traceability**

| Class Name        | **Requirement ID                  |
|:---------------------:|:--------------------------------------:|
| classCustomer         | FR1, FR2, NFR1, NFR3                   |
| classPaymentGateway   | FR17, FR18, NFR5                 |
| classAccount          | FR28, FR31, NFR1, NFR3, NFR5           |
| classBank             | FR17, FR31, NFR1, NFR2                 |
| classAuthentication   | FR6, FR7, FR11, NFR1, NFR3, NFR5       |
| Transaction           | FR22, FR24, NFR5                 |


# Software Artifacts
This section is a description of all the artifacts linked to this project. It contains hyperlinks that redirect one to each of those artifacts.


* [Use Case Diagram 1](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Use%20Case%20Diagram%201.pdf)
* [Use Case Diagram 2](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Use%20Case%20Diagram%202.pdf)
* [Use Case Diagram 3](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Use%20Case%20Diagram%203.pdf)
* [Windows nav](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Windows%20nav.%20assgt.pdf)
* [crcCard](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/crcCard.pdf)
* [Activity Diagram-2](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Activity_Diagram-2.pdf)
* [Activity Diagram-3](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/Activity_Diagram-3.pdf)
* [ClassDiagrams](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/ClassDiagrams.pdf)
* [Gantt Chart](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/GanttChart.pdf)
* [PreconsPostcons](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/PreconsPostcons.pdf)
* [SystemOverview](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/b5672212917dbb2c49447867736538cd94aa5e03/artifacts/artifacts/SystemOverview.pdf)
* [Presentation Slides to PDF](https://github.com/KawiraSharon/GVSU-CIS641-Soloscribe/blob/0d19b89913a7769e631557692a10ac1e6169f11a/docs/Semester_Project_Presentation_Slides_to_PDF.pdf)



Please note that the project was implemented as a two-course project. Please see below the features implemented for this course; CIS 641, Systems Analysis and Design, versus the features implemented for course CIS611, Introduction to Software Engineering.

Features Implemented for Course CIS 641
- Sign Up, Sign In, Sign Out
- Total Balance
- Transaction Overview
- All Transactions
- Transfer Funds Functionality
- Personalizing User Experience with a “Welcome <first name>” message 
- Dwolla API Integration to ensure smooth and seamless money transfers

Features Implemented for course CIS 611
- See All Transactions
- Bank Accounts
- Link Bank Account
- Transaction Classifications
- Add Banking Account
- SSR Authentication for linking another bank account using Plaid
- Plaid and Dwolla Integration to handle multiple bank accounts and transactions
