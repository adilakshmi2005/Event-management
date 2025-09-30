
Event Registration Management System
This project is a Salesforce-based solution to help organizations manage event registrations, attendee feedback, and event performance efficiently. It was built using Salesforce Admin + Developer features with automation, dashboards, and secure role-based access.
Project Overview
•	Event Registration – Attendees can register for upcoming events with role-based access.
•	Feedback Collection – Submit post-event feedback with ratings and comments.
•	Event Management – Create and manage events with capacity, date, time, location, and department targeting.
•	Automation – Registration confirmation emails, feedback acknowledgments, duplicate checks, and capacity enforcement.
•	Reports & Dashboards – Event-wise registrations, department-wise participation, feedback summaries, upcoming events overview.
Salesforce Features Used
•	Custom Objects: Event__c and Attendee__c
•	Record Types & Page Layouts: Event Registration vs Event Feedback
•	Validation Rules: Event required, valid phone/email, feedback only after event date, capacity enforcement
•	Profiles & Roles: Event Admin (full access), User/Attendee (self-service registration & feedback)
•	Flows for automation: registration/feedback emails, duplicate checks, capacity full alerts
•	Reports & Dashboards for real-time monitoring: registration trends, feedback ratings, department insights
Testing Summary
•	Attendee registration → Sends registration confirmation email
•	Duplicate registration attempt → Blocked successfully
•	Event capacity limit → Registration blocked when full
•	Feedback submission → Only allowed after event date
•	Validation rules → Block invalid emails, phone numbers, missing events
•	Reports & Dashboards → Accurately reflect registrations, feedback, and departmental participation

Future Enhancements
•	Public-facing registration portal (Experience Cloud)
•	Online payment integration (Razorpay/Stripe) for paid events
•	Mobile app support (Salesforce Mobile / LWCs) for attendees and organizers
•	Smart analytics for attendee participation and feedback trends
•	Waitlist functionality for full events

Author
chinnasamireddy1234@gmail.com

