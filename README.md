# HMIS Analytics Dashboard

A lightweight, client-side analytics dashboard that transforms raw HMIS Program Performance Report (PPR) exports into an interactive and user-friendly reporting experience.

Instead of digging through thousands of rows in Excel, this dashboard allows users to upload an HMIS PPR export and immediately explore trends, demographics, housing outcomes, provider performance, and data quality metrics through interactive charts and filters.

---

## Overview

HMIS reports contain a large amount of valuable information, but the standard Excel output can be difficult for program managers, directors, supervisors, and analysts to interpret.

This project was created to:

- Make HMIS data easier to understand
- Reduce time spent filtering and analyzing spreadsheets
- Provide visual dashboards for decision making
- Identify trends across programs and populations
- Surface data quality issues before reporting deadlines
- Allow non-technical staff to explore HMIS reporting data

The dashboard runs entirely in the browser and requires no backend infrastructure.

---

## Features

### Excel File Upload

- Drag-and-drop upload interface
- Supports `.xlsx` and `.xls` files
- Automatic workbook parsing
- Multi-sheet workbook support
- Sheet selection when multiple worksheets exist
- Client-side processing only

### Fiscal Year Analysis

Automatically detects:

- Fiscal year boundaries
- Fiscal quarters
- Reporting periods

Users can analyze data by:

- Total Fiscal Year
- Fiscal Quarter (Q1-Q4)
- Custom Date Range

### Interactive Filters

Filter data by:

- Provider
- Veteran Status
- Gender
- Race & Ethnicity
- Age Group
- Disabling Condition
- Exit Destination
- Housing Placement Status

Features include:

- Multi-select filters
- Active filter badges
- Quick removal of individual filters
- One-click clear all
- Click-to-filter charts and tables

---

## Dashboard Sections

### Overview

Provides high-level metrics including:

- Unique Clients Served
- Newly Served Clients
- Unique Veterans
- Unique Leavers
- Positive Placements
- Permanent Housing Exits
- Average Length of Stay
- Average Age at Entry
- Active Providers

### Provider Breakdown

Compare providers across:

- Total clients served
- Quarterly enrollment activity
- Newly served clients
- Housing placements
- Permanent housing exits
- Placement rates
- Average length of stay

Clicking a provider automatically filters the dashboard.

### Demographics

Interactive charts for:

#### Gender

Displays:

- Client counts
- Percentages
- Distribution across gender identities

#### Age Groups

Breaks clients into HMIS reporting age ranges.

#### Race & Ethnicity

Visualizes population composition across race and ethnicity categories.

#### Veteran Status

Analyzes veteran and non-veteran populations.

#### Disabling Condition

Displays disabling condition classifications and reporting completeness.

### Housing Outcomes

Tracks:

- Exit destinations
- Permanent housing outcomes
- Temporary housing outcomes
- Institutional exits
- Homeless exits
- Other outcomes

Additional visualizations include:

- Veteran vs. non-veteran outcomes
- Length of stay distributions
- Average length of stay comparisons
- Exit destination trends

### Trends

Quarter-over-quarter reporting for:

- People served
- Newly served clients
- Housing placements
- Veterans served
- Average length of stay

### Data Quality

Evaluates completeness of key HMIS fields:

- Entry Date
- Exit Date
- Exit Destination
- Age
- Gender
- Race & Ethnicity
- Veteran Status
- Disabling Condition
- Provider

Fields are categorized as:

- Good
- Fair
- Poor

This helps identify reporting gaps before submitting official reports.

---

## Provider Management

When loading a report, users can choose which providers to include in the analysis.

Features include:

- Provider inclusion/exclusion
- Session-based filtering
- On-demand provider management after loading
- Automatic dashboard recalculation

---

## Data Validation

The dashboard validates file structure before loading.

Checks include:

- Required column detection
- Missing field identification
- Reporting impact warnings
- Critical field validation

Users receive clear explanations when columns are missing and can choose whether to continue.

---

## Privacy & Security

This application runs entirely inside the browser.

### No Data Leaves Your Computer

✅ No server

✅ No database

✅ No cloud storage

✅ No API calls containing client data

✅ No user tracking

✅ Local Excel processing only

All uploaded files remain on the user's device.

---

## Technology Stack

### Frontend

- HTML5
- CSS3
- Vanilla JavaScript

### Libraries

- SheetJS (XLSX)
- Chart.js

### Design Principles

- No backend required
- No build process
- No framework dependencies
- Portable single-file application
- Works entirely offline after libraries are loaded

---

## Expected HMIS Columns

The dashboard is designed around HMIS PPR exports and expects fields similar to:

- Client Unique Id
- HMIS Provider
- Entry Date
- Exit Date
- Length of Stay (Leavers in FY)
- Exit Destination
- Exit Destination Crosswalk
- Newly Served in FY
- Placed in FY
- Age at Entry
- Age Breakout
- Gender
- Race and Ethnicity
- Veteran Status
- Disabling Condition
- Household ID

Column validation occurs automatically during upload.

---

## Installation

No installation

---

## Privacy Considerations

This project was intentionally designed without sample datasets or screenshots.

Because the dashboard is used to analyze HMIS Program Performance Reports (PPRs), example outputs may contain sensitive client, demographic, housing, or program information.

To protect client privacy and maintain compliance with organizational data handling practices:

- No sample HMIS datasets are included
- No screenshots of production data are included
- No client information is stored by the application
- All processing occurs locally within the user's browser

Users should only load reports that they are authorized to access and analyze.
