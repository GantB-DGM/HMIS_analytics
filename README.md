HMIS Analytics Dashboard

A lightweight, client-side analytics dashboard for transforming raw HMIS Program Performance Report (PPR) exports into an interactive, user-friendly reporting experience.

Instead of digging through thousands of rows in Excel, this dashboard allows users to upload an HMIS PPR export and immediately explore trends, demographics, housing outcomes, provider performance, and data quality metrics through interactive charts and filters.

Why This Exists

HMIS reports contain a large amount of valuable information, but the default Excel output can be difficult for program managers, directors, and frontline supervisors to interpret.

This tool was created to:

Make HMIS data easier to understand
Reduce time spent filtering spreadsheets
Provide visual dashboards for decision making
Identify trends across programs and populations
Surface data quality issues before reporting deadlines
Allow non-technical staff to analyze PPR data without Excel expertise
Features
Interactive Data Upload
Drag-and-drop Excel upload
Supports .xlsx and .xls
Multi-sheet workbook detection
Automatic sheet selection
Client-side processing (no data leaves your computer)
Fiscal Year Analysis

Automatically detects:

Fiscal year boundaries
Fiscal quarters
Reporting period date ranges

Provides:

Full Fiscal Year view
Quarter-by-quarter analysis
Custom date range filtering
Dashboard Overview

Quickly see:

Unique clients served
Newly served clients
Veteran counts
Unique leavers
Positive housing placements
Permanent housing exits
Average length of stay
Average age at entry
Active providers
Advanced Filtering

Filter data by:

Provider
Veteran status
Gender
Race & ethnicity
Age group
Disabling condition
Exit destination
Housing placement status

Features include:

Multi-select filtering
Active filter badges
Filter tags
One-click filter removal
Cross-dashboard filtering
Provider Analysis

Compare providers across:

Total clients served
Quarterly activity
Newly served clients
Housing placements
Permanent housing outcomes
Placement rates
Average length of stay

Click any provider row to immediately filter the dashboard.

Demographics Dashboard

Interactive visualizations for:

Gender

Horizontal bar charts showing:

Client counts
Percentages
Distribution across gender identities
Race & Ethnicity

Doughnut charts showing:

Population composition
Relative representation
Veteran Status

Breakdowns of:

Veteran populations
Non-veteran populations
Disability Status

Analysis of:

Disabling conditions
Missing or unknown responses
Age Groups

Age band analysis using HMIS age classifications.

Housing Outcomes Dashboard

Analyze:

Exit destinations
Permanent housing placements
Temporary housing placements
Institutional exits
Homeless exits
Other outcomes

Additional insights include:

Veteran vs. non-veteran outcomes
Length of stay distributions
Average length of stay comparisons
Exit destination breakdowns
Quarterly Trend Analysis

Track changes over time:

Clients served
Newly served clients
Housing placements
Veteran participation
Length of stay metrics

Visualized using:

Line charts
Trend comparisons
Quarter-over-quarter reporting
Data Quality Monitoring

Identify fields that need attention.

Measures completeness for:

Entry Date
Exit Date
Exit Destination
Age
Gender
Race & Ethnicity
Veteran Status
Disabling Condition
Provider

Automatically categorizes fields as:

Good
Fair
Poor

Helping programs improve reporting quality before submitting reports.

Privacy & Security

This application runs entirely in the browser.

✅ No server required

✅ No client data uploaded

✅ No database

✅ No external storage

✅ Data remains on the user's machine

Excel files are processed locally using SheetJS.

Technology Stack
Frontend
HTML5
CSS3
Vanilla JavaScript
Libraries
SheetJS (xlsx)
Chart.js

No build process, backend, framework, or installation required.

Expected HMIS Columns

The dashboard is designed for HMIS Program Performance Report (PPR) exports and expects fields such as:

Client Unique Id
HMIS Provider
Entry Date
Exit Date
Length of Stay
Exit Destination
Newly Served Indicators
Housing Placement Indicators
Age
Gender
Race and Ethnicity
Veteran Status
Disabling Condition
Household ID

The application validates headers during upload and clearly identifies missing columns that may impact reporting.

How To Use
Export a Program Performance Report (PPR) from HMIS
Save the report as Excel (.xlsx)
Open the dashboard
Drag the file into the upload area
Select the appropriate worksheet (if applicable)
Choose which providers to include
Explore the dashboard
Intended Audience

This tool is useful for:

HMIS Administrators
Program Managers
Shelter Directors
Data Analysts
Grants & Compliance Teams
Executive Leadership
Continuum of Care reporting staff
Future Enhancements

Potential future improvements include:

Export filtered results
PDF report generation
Saved filter presets
Benchmark comparisons
Historical year-over-year analysis
KPI scorecards
Program-specific dashboards
Custom provider groupings
Disclaimer

This dashboard is designed to improve accessibility and analysis of HMIS PPR data. All metrics are calculated from the uploaded report and should be reviewed alongside official HMIS reporting standards and guidance when used for compliance or grant reporting.

Built to make HMIS data easier to understand, analyze, and act on. 📊🏠📈
