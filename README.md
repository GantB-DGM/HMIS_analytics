# HMIS Analytics Dashboard

A lightweight, privacy-first analytics dashboard that transforms raw HMIS Program Performance Report (PPR) exports into an interactive and user-friendly reporting experience.

All processing occurs locally in the browser, allowing organizations to analyze sensitive HMIS reporting data without uploading information to external systems.

Instead of digging through thousands of rows in Excel, users can upload a PPR export and immediately explore trends, demographics, housing outcomes, provider performance, and data quality metrics through interactive charts and filters.

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

This application runs entirely inside the user's web browser.

### No Data Leaves Your Computer

✅ No server infrastructure

✅ No database

✅ No cloud storage

✅ No user accounts

✅ No analytics or telemetry

✅ No external transmission of client data

✅ Local Excel processing only

All uploaded files remain on the user's device and are never sent to a server.

---

## Privacy Considerations

This project was intentionally designed with a privacy-first approach.

Because the dashboard analyzes HMIS Program Performance Reports (PPRs), the underlying data may contain sensitive information related to clients, demographics, housing outcomes, program participation, and service utilization.

To protect client confidentiality and support responsible data handling practices:

- No sample HMIS datasets are included with this project
- No screenshots containing production data are included in this repository
- No uploaded data is stored by the application
- No client information is transmitted to external systems
- No analytics, tracking, or telemetry are collected
- All processing occurs locally within the user's web browser

Users should only load HMIS reports they are authorized to access and review.

### Privacy-First Design Principles

- Client-side processing only
- No backend services required
- No database dependencies
- No cloud storage
- No user accounts
- No persistent data retention
- Designed to support secure analysis of HMIS reporting data

This application is intended to improve accessibility and understanding of HMIS reporting data while minimizing privacy risks associated with handling sensitive client information.

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

No installation required.

Download the HTML file and open it in a web browser.

Alternatively, host it on any web server:

```bash
git clone https://github.com/your-org/hmis-analytics-dashboard.git
```

Open:

```text
index.html
```

---

## Usage

1. Export a Program Performance Report (PPR) from HMIS.
2. Save the report as an Excel file.
3. Open the dashboard.
4. Upload the file.
5. Select the correct worksheet if multiple sheets are present.
6. Choose which providers to include.
7. Explore the dashboard using tabs, charts, and filters.

---

## Intended Audience

This tool is useful for:

- HMIS Administrators
- Program Managers
- Shelter Managers
- Data Analysts
- Compliance Staff
- Grant Writers
- Executive Leadership
- Continuum of Care Reporting Teams

---

## Future Enhancements

Potential future improvements include:

- CSV export
- PDF report generation
- Saved filter presets
- Historical year-over-year comparisons
- KPI scorecards
- Grant reporting views
- Benchmark comparisons
- Custom provider groupings
- Additional HMIS report support

---

## Disclaimer

This dashboard is intended to improve accessibility and analysis of HMIS Program Performance Report (PPR) data.

While calculations are based directly on uploaded report data, official HMIS guidance and reporting standards should always be referenced when using this information for compliance, funding, regulatory reporting, or audit purposes.

---

## License

- Internal Use Only

---

**Built to make HMIS data easier to understand, analyze, and act on while keeping sensitive data on the user's device.**
