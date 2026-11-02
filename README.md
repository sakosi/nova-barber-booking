# Nova Barber Studio — Smart Booking System

A web-based appointment booking system powered by n8n automation, Google Calendar, and Google Sheets.

The project demonstrates how a small business can automate its appointment scheduling process through a custom booking interface and an integrated backend workflow.

## Project Overview

Nova Barber Studio is a demo booking platform designed for a fictional barbershop.

Customers can submit appointment requests through a responsive website. The backend automatically validates booking details, checks service availability, verifies the requested time slot, creates calendar events, and stores booking information.

## Features

### Frontend
- Responsive booking website.
- Service selection.
- Appointment date and time selection.
- Customer information form.
- JavaScript-based HTTP requests.

### Backend Automation
- Webhook-based request processing.
- Data cleaning and normalization.
- Customer information validation.
- Automatic service lookup.
- Dynamic service duration calculation.
- Business-hours validation.
- Google Calendar availability checking.
- Automatic appointment creation.
- Booking conflict detection.
- HTTP response handling.

### Integrations
- **n8n:** Workflow automation and backend logic.
- **Google Calendar API:** Appointment availability and event creation.
- **Google Sheets API:** Booking database and service management.
- **GitHub Pages:** Static website hosting.

## Workflow Architecture

```text
Customer Booking Form
        |
        v
     Webhook
        |
        v
  Data Normalization
        |
        v
   Service Lookup
        |
        v
   Booking Validation
        |
        v
 Calendar Availability
        |
        v
   Slot Validation
        |
        v
 Create Calendar Event
        |
        v
  Save Booking to Sheets
        |
        v
  Booking Confirmation
```

Invalid requests and unavailable appointment slots are handled through separate response branches.

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Website structure |
| CSS3 | Responsive interface |
| JavaScript | Frontend logic and data processing |
| n8n | Workflow automation |
| REST API | Service communication |
| JSON | Data exchange |
| Google Calendar API | Appointment scheduling |
| Google Sheets API | Booking storage |
| GitHub Pages | Frontend hosting |

## Project Structure

```text
nova-barber-booking/
├── index.html
├── README.md
├── workflow/
├── screenshots/
└── docs/
```

## Testing

The booking workflow has been tested with:

- Successful appointment submissions.
- Service lookup and duration calculation.
- Google Calendar availability checks.
- Appointment creation.
- Google Sheets record creation.
- Unavailable time-slot handling.
- Invalid booking submissions.

## Project Status

**Working MVP**

The core booking workflow has been demonstrated successfully.

Planned improvements:
- Appointment cancellation.
- Appointment rescheduling.
- Automated email reminders.
- Booking management interface.
- Enhanced webhook security.
- Protection against simultaneous booking conflicts.

## Security Notes

- API credentials must be configured separately.
- Private customer information must not be published.
- Webhook endpoints should be protected before production deployment.
- The exported workflow should not contain access tokens, passwords, or private credentials.

## Project Purpose

This project demonstrates practical skills in workflow automation, frontend development, API integrations, data validation, and business process automation.

It was developed as a portfolio project to demonstrate how automation can reduce manual appointment management for small businesses.
