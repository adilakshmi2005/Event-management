# Event Registration & Feedback Management System

# Project Overview

The **Event Registration & Feedback Management System** is a Salesforce-based solution developed to digitize and centralize the entire event organization process.
It simplifies how event coordinators manage event creation, attendee registration, communication, and performance tracking — all within one Salesforce platform.

# Goal:
To streamline event management by automating registration, confirmation, and reporting processes — reducing manual errors and improving operational efficiency.

# Key Features:

Event Managers can create, edit, and track events easily.
Attendees can register quickly without duplication.
Automatic confirmation and feedback emails are sent through Salesforce Flows.
Real-time dashboards and reports provide actionable insights on participation and event performance.

# Phase 1: Problem Understanding & Industry Analysis

# Problem Statement

Event organizers often face challenges such as:

* Manual attendee registration using spreadsheets or paper forms
* Lack of automated communication with attendees
* Difficulty in tracking event capacity and attendance
* No centralized dashboard to view event analytics

# Solution

A Salesforce-based centralized system to:

Manage Events and Attendees using custom objects
Create relationships between events and attendees
Automate confirmation and feedback emails via Flows & Email Alerts
Provide real-time dashboards for event insights and analysis

# Phase 2: Org Setup & Configuration

  Created a Salesforce Developer Org
  Enabled Lightning Experience
  Configured Custom Tabs**, App Launcher Access, and Object Permissions
  Created a Custom Profile – Event_Admin with full CRUD access to manage events and attendees
  

# Phase 3: Data Modeling & Relationships

# Custom Objects

Event__c → Stores event details (Name, Date, Location, Capacity, Type)
Attendee__c → Stores attendee details (Name, Email, Phone, Department, Registered Event)

# Relationships

Lookup Relationship: Attendee → Event
  (Each attendee is linked to a specific event)

#  Phase 4: Process Automation (Admin)

* Built a **Record-Triggered Flow** on Attendee creation
* Added logic to **prevent duplicate registrations** (based on name and email)
* Configured **Email Alerts** connected to the Flow
* Created **Classic Email Templates** for:

  * Registration Confirmation
  * Feedback Acknowledgment

---

# Phase 5: Apex Programming (Developer)

Currently, no Apex customization is used in this version.
However, for **future enhancement**, the following are planned:

Apex Class for bulk registration import
Apex Trigger for event capacity validation

# Phase 6: User Interface Development

* Created Tabs for Event and Attendee objects
* Customized Page Layouts for different record types:

  Event Registration Layout
  Event Feedback Layout
* Added Lookup fields to connect attendees with specific events
* Designed a user-friendly navigation flow within the Salesforce App

# Phase 7: Integration & External Access

# Current Scope:

* Application runs completely within Salesforce.

# Future Scope:

* Integration with Eventbrite, Google Calendar, or other external event management tools.

# Phase 8: Data Management & Deployment

* Loaded sample data for Events and Attendees
* Maintained version control and documentation via GitHub
* Deployment possible using Change Sets or Salesforce DX (SFDX)

# Phase 9: Reporting, Dashboards & Analytics

# Reports:

* Event-wise Department-wise Summary
* Event Capacity vs Registrations
* Event Registration Summary
* Department-wise Registrations
* Upcoming Events List

# Dashboards:

1. **Department Insights Dashboard** – shows participation of different departments across events
2. **Event Overview Dashboard** – visualizes event-wise capacity, registration count, and upcoming events

#  Future Scope / Enhancements

* Event capacity validation and **waitlist feature**
* Integration with **payment gateways** for paid events
* **Experience Cloud Portal** for attendee self-registration
* Mobile-friendly **LWC component** for direct registration
* Automated **post-event survey** collection and analytics

# Author

Samireddi Adilakshmi
B.E. Information Technology
India


