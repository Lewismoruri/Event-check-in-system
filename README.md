# Event Check-In System

A simple event registration and check-in prototype built with Google Forms and Google Sheets.

The project explores how a lightweight, collaborative workflow can be used to manage event registration, attendee check-in, and basic attendance analysis without relying on paper-based lists.

## Overview

Event registration and check-in can become time-consuming when attendees have to be searched for manually on printed lists.

I started this project as a small experiment to explore whether Google Forms and Google Sheets could provide a simpler way to manage the process.

The prototype follows this workflow:

**Registration Form → Responses → Check-In → Attendance Data → Dashboard**

The project uses synthetic/test data for demonstration purposes.

## Features

### Registration

A Google Form is used to collect attendee information.

The submitted responses are automatically stored in Google Sheets, providing a central source of registration data.

### Attendee Check-In

A separate check-in workspace is used to manage attendees.

The current prototype tracks:

- Full Name
- Email
- Check-In Status
- Check-In Time

Check-in status can be updated between:

- `Checked_In`
- `Not Checked In`

The check-in time is recorded when an attendee arrives.

### Attendance Dashboard

The check-in data is used to generate basic attendance insights, including:

- Total Registered
- Total Attended
- Did Not Attend
- Attendance Rate
- Attendance breakdown
- Arrival progression

This demonstrates how operational data collected during an event can also be turned into useful information for understanding attendance.

## Project Structure

```text
Registration Form
       ↓
Google Form Responses
       ↓
Guest Check-In
       ↓
Check-In Status + Time
       ↓
Attendance Dashboard
