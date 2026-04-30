# 369_Project
Azure requirements Doc + Grabdocs Testing Repo From Bai Kebbie-Anthony

https://kebbieanthonybai.atlassian.net/jira/software/projects/GTA/summary

📄 Web Testing Requirements Document

-Project Overview-

This document defines the testing requirements for validating the functionality of:

Scheduling and joining meetings
Group messaging
@mention functionality and responses

The goal is to ensure all features work correctly in a web environment before deployment.

  -Objectives-
  
Meeting scheduling
Joining meetings
Sending messages in group chat
Mentioning users (@username)
Receiving and responding to mentions

 -Test Environment-
 
Platform: GrabbDocs on a web browser (Chrome) 
Tool: Selenium
Issue Tracking: Jira

 -Features to be Tested-

4.1 Schedule Meeting

Test Cases:
Create a meeting with valid inputs
Create a meeting with missing fields
Verify meeting link generation
Verify the meeting appears in the user dashboard

Expected Results:
The meeting is successfully created
Errors shown for invalid input

4.2 Join Meeting

Test Cases:
Join with a valid meeting link
Join with an invalid meeting ID
Join without authentication (if restricted)

Expected Results:
User joins successfully with a valid link
An error was displayed for an invalid meeting

4.3 Group Messaging

Test Cases:
Send a message in the group chat
Verify message visibility to all users
Refresh page → verify message persistence

Expected Results:
Messages appear instantly
Messages are stored and reloaded

4.4 @Mention Functionality

Test Cases:
Mention a valid user (@username)
Mention a non-existent user
Multiple mentions in one message

Expected Results:
Mention is highlighted
Valid user receives notification
Invalid mention shows an error or no action

4.5 Response to Mentions

Test Cases:
Tagged user replies to the message
Verify reply visibility to the group
Verify message order

Expected Results:
Reply appears correctly
Conversation flow is maintained

  -Acceptance Criteria-
All critical test cases pass
No major defects remain open
Core features function without failure

 -Defect Tracking-
All bugs should be logged in Jira with:
Title
Steps to reproduce
Expected vs actual result
Severity (Low, Medium, High)
