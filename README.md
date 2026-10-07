# Event Check-In System

A simple event registration, check-in, and attendance tracking prototype built with Google Forms and Google Sheets.

## Overview

Event check-in can become time-consuming when attendees have to be searched for manually on printed lists or through large spreadsheets.

I started this project as a small experiment to explore whether commonly available tools such as Google Forms and Google Sheets could be used to create a simpler check-in workflow.

The prototype connects event registration, attendee check-in, and attendance analysis into one workflow.

### Workflow

**Registration Form → Form Responses → Guest Check-In → Attendance Data → Dashboard**

The project currently uses synthetic/test data for demonstration purposes.

---

## Project Objectives

The main objectives of this prototype are to:

- Create a simple event registration process
- Capture attendee information digitally
- Provide a separate workspace for checking attendees in
- Record check-in status and time
- Calculate basic attendance metrics
- Turn attendance data into a simple dashboard
- Explore ways to make event check-in faster and easier for volunteers

---

## How It Works

### 1. Registration

The process begins with a Google Form used to collect attendee information.

When a person submits the form, their response is automatically stored in Google Sheets.

The Google Form acts as the registration point, while the responses provide the source data for the rest of the workflow.

---

### 2. Form Responses

The submitted registration information is stored in a Google Sheets response sheet.

This sheet acts as the raw/source data and is kept separate from the volunteer-facing check-in workspace.

This separation helps prevent the raw registration data from being unnecessarily modified during the check-in process.

---

### 3. Guest Check-In

A separate `Guest Check_In` sheet is used as the check-in workspace.

The current prototype includes:

- Full Name
- Email
- Check-In Status
- Check-In Time

The check-in status uses a dropdown with two options:

- `Checked_In`
- `Not Checked In`

When an attendee arrives, their status can be updated and their check-in time recorded.

The goal is to keep this workspace focused on the information needed to identify and check in an attendee.

---

### 4. Attendance Dashboard

The check-in information can then be used to generate basic attendance insights.

The current dashboard includes:

- Total Registered
- Total Attended
- Did Not Attend
- Attendance Rate
- Attendance breakdown
- Guest arrival progression

This demonstrates how information collected during an event can be transformed from simple operational records into useful attendance insights.

---

## Tools Used

- **Google Forms** — event registration and data collection
- **Google Sheets** — data storage, check-in workflow, calculations, and dashboard
- **Data Validation** — check-in status dropdown
- **Spreadsheet Formulas** — attendance calculations
- **Charts & Dashboards** — visualizing attendance information

---

## Project Structure

The prototype is organized around three main areas:

```text
Google Form
     │
     ▼
Form Responses
     │
     ▼
Guest Check_In
     │
     ├── Check-In Status
     └── Check-In Time
     │
     ▼
Attendance Dashboard
