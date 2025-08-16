# EventEase: Power Automate
# Event Management & Certificate Automation System

![alt text]([http://url/to/img.png](https://github.com/devlop-suraj/EventEase/blob/main/ss.png))

Workflow Overview
Goal: Automate registration, attendance, and certificate distribution while adding analytics & AI features.
Workflow – Microsoft Forms Based
(https://github.com/devlop-suraj/EventEase/blob/main/ss.png)
1. Registration Phase
1.	Participant Registration
o	Fill Microsoft Form with fields: Name, Email, College, Role (Student/Faculty/etc.).
2.	Trigger in Power Automate
o	Trigger: When a new response is submitted (Microsoft Forms connector).
o	Action: Get response details.
3.	Store Data
o	Save participant details in SharePoint List (or Excel in OneDrive for Business).
4.	Confirmation Email
o	Power Automate sends a personalized confirmation email with:
	Event details
	Unique QR Code (generated via QR Code API or Encodian connector).
________________________________________
2. Pre-Event Preparation
•	Power BI dashboard auto-updates from the SharePoint List:
o	Registrations by category
o	Total count
o	College-wise breakdown
________________________________________
3. Event Day Check-In
•	Volunteers use Power Apps mobile app:
o	Scan participant QR code
o	Power Automate updates the “Attendance” column in SharePoint to Present.
•	Power BI dashboard shows real-time attendance.
________________________________________
4. Post-Event Certificate Distribution
1.	Scheduled Flow in Power Automate triggers after the event ends.
2.	Condition: If Attendance = Present, proceed.
3.	Merge participant name into a Word Online (Business) certificate template.
4.	Convert the document to PDF.
5.	Send personalized participation certificate via email.
________________________________________
Tools & Connectors Used
•	Microsoft Forms – Registration form
•	SharePoint List – Data storage
•	Power Automate – Workflow automation
•	Power Apps – QR Code scanning app
•	QR Code API – QR code generation
•	Word Online (Business) – Certificate creation
•	Power BI – Event analytics
________________________________________
If you want, I can now design the professional architecture diagram showing:
•	Microsoft Forms → Power Automate → SharePoint → Power Apps → Power BI → Certificates
