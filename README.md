### ITSM-Ticket-Management

#### Problem Statement:
ABC Tech is a mid-size organisation operation in IT-enabled business segment over a decade. On an average ABC Tech receives 22-25k IT incidents/ tickets, which were handled to best practice ITIL framework with incident management, problem management, change management and configuration management processes. These ITIL practices attained matured process level and recent audit confirmed that further improvement initiatives may not yield return of investment.<br>
ABC Tech management is looking for ways to improve the incident management process as recent customer survey results shows that incident management is rated as poor.<br>
Machine Learning as way to improve ITSM processes<br>
ABC Tech management recently attended Machine Learning conference on ML for ITSM.<br>
Machine learning looks prospective to improve ITSM processes through prediction and automation. They came up with 4 key areas, where ML can help ITSM process in ABC Tech.<br>
1.	Predicting High Priority Tickets: To predict priority 1 & 2 tickets, so that they can take preventive measures or fix the problem before it surfaces.<br>
2.	Forecast the incident volume in different fields, quarterly and annual. So that they can be better prepared with resources and technology planning.<br>
3.	Auto tag the tickets with right priorities and right departments so that reassigning and related delay can be reduced.<br>
4.	Predict RFC (Request for change) and possible failure /misconfiguration of ITSM assets.<br>

#### Domain Analysis:
1.	Configuration Item Name: A Configuration Item (CI) is a component or asset within an IT system that needs to be managed, tracked, and controlled. Examples of CIs might include hardware devices, software applications, network components, or even people and processes.<br>
2.	CI_Cat: In ITSM refers to the category or classification of a specific Configuration Item. The category might be used to group similar CIs together for easier management and tracking, or to help identify the type of CI and its function within the IT environment.<br>
3.	CI_Subcat: This column refers to the CI subcategory, which is a further classification of the CI within its category. Examples of CI subcategories include server, desktop, laptop, operating system, and application.<br>
4.	WBS: This column refers to the Work Breakdown Structure (WBS), which is a hierarchical decomposition of the project into smaller, more manageable components. The WBS is used to organize and track the work required to complete the project.<br>
5.	Incident_ID: This column refers to the unique identification number assigned to the incident. This number is used to track and manage the incident throughout its lifecycle.<br>
6.	Status: This column refers to the current status of the incident. Examples of status include new, in progress, resolved, and closed.<br>
7.	Impact: This column refers to the degree of impact the incident has on the business. The impact is usually measured in terms of the number of users affected and the level of disruption to business operations.<br>
8.	Urgency: This column refers to the degree of urgency required to resolve the incident. Urgency is usually measured in terms of the business impact and the severity of the issue.<br>
9.	Priority: This column refers to the priority level assigned to the incident. The priority is usually determined based on the impact and urgency of the incident, as well as other factors such as customer requirements and contractual obligations.<br>
10.	number_cnt: This column refers to the number of times the incident has been logged or recorded.<br>
11.	Category: This column refers to the category of the incident, which is a way to classify the type of issue being reported. This can include categories such as hardware, software, network, user, and more.<br>
12.	KB_number: This column refers to the knowledge base (KB) article number associated with the incident. A knowledge base is a centralized repository of information that contains solutions to common issues and troubleshooting guides.<br>
13.	Alert_Status: This column refers to the status of any alerts associated with the incident. Alerts are notifications generated by a monitoring system that detect and report on events or issues.<br>
14.	No_of_Reassignments: This column refers to the number of times the incident has been reassigned to a different team or individual for further investigation or resolution.<br>
15.	Open_Time: This column refers to the date and time when the incident was initially opened or reported.<br>
16.	Reopen_Time: This column refers to the date and time when the incident was reopened after being closed previously.<br>
17.	Resolved_Time: This column refers to the date and time when the incident was resolved, meaning the issue has been identified and a solution has been implemented.<br>
18.	Close_Time: This column refers to the date and time when the incident was closed, meaning the issue has been fully resolved and no further action is required.<br>
19.	Handle_Time_hrs: This column refers to the total time in hours that was spent working on the incident. This includes the time spent investigating, troubleshooting, and resolving the issue.<br>
20.	Closure_Code: This column refers to the code or reason used to close the incident. This can include codes such as "resolved," "closed by user," "no fault found," and more.<br>
21.	No_of_Related_Interactions: This column refers to the number of related interactions associated with the incident. Related interactions can include things like phone calls, emails, or chat messages related to the incident.<br>
22.	Related_Interaction: This column refers to the specific interaction or communication associated with the incident.<br>
23.	No_of_Related_Incidents: This column refers to the number of related incidents associated with the incident being reported.<br>
24.	No_of_Related_Changes: This column refers to the number of related changes associated with the incident being reported. Changes can include things like updates to software, hardware upgrades, or modifications to IT infrastructure.<br>
25.	Related_Change: This column refers to the specific change or modification associated with the incident being reported.<br>

#### Summary:
The project is done with the purpose of:

* Finding out factors which affects priority and training a model which accurately predicts it so that preventive measures can be taken for High Priority Tickets and reassigning can be reduced.
* Finding out factors which affect RFC and predicting it.
* Forecasting Incident Volume in the future so that they can be better prepared with resources and technology planning.<br>

The following steps are carried out:

* Importing the data, necessary libraries, & exploring the data to look for missing values.
* Selecting the features for analysis, label encoding the ordinal column and splitting the data into test & train.
* Training the data using algorithms like Support Vector Machine, Decision Tree, Random Forest, K-Nearest Neighbor, XGBoost Classifier and Artificial Neural Network and checking the accuracy to find out which algorithm is the best.
* Exporting the model with highest accuracy.
* For Incident Volume Forecasting, Ticket Opening Time is taken and Time Series Forecasting is used.
