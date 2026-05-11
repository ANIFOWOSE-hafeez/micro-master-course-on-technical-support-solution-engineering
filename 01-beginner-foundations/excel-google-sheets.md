# Excel / Google Sheets

> Learn spreadsheet skills like a real Technical Support Engineer or Solution Engineer.

Spreadsheets are one of the most underrated technical tools in startups.

Even senior engineers, operations teams, customer success teams, support managers, solution engineers, and founders use spreadsheets daily for:
- tracking incidents
- managing assets
- analyzing support tickets
- reporting uptime
- documenting infrastructure
- handling onboarding
- monitoring KPIs
- exporting logs
- auditing systems

If you become extremely good with spreadsheets, you immediately become more valuable operationally.

---

# Learning Goals

By the end of this lesson, learners should understand:

- spreadsheet fundamentals
- rows, columns, and cells
- formulas and functions
- filtering and sorting
- conditional formatting
- data validation
- ticket tracking workflows
- operational reporting
- startup support dashboards
- CSV handling
- basic analytics
- automation-ready spreadsheet thinking

---

# What Are Excel and Google Sheets?

They are spreadsheet applications used to:
- organize data
- analyze information
- calculate metrics
- track operations
- generate reports

---

# Difference Between Excel and Google Sheets

| Excel | Google Sheets |
|---|---|
| Desktop-first | Cloud-first |
| Advanced enterprise features | Easier collaboration |
| Powerful offline support | Real-time collaboration |
| Common in enterprises | Common in startups |

---

# Startup Reality

Many startups heavily use:
- Google Workspace
- Google Sheets
- Notion
- Airtable

because collaboration is critical.

---

# Real Startup Use Cases

Support teams use spreadsheets for:

| Use Case | Example |
|---|---|
| Ticket tracking | SLA monitoring |
| Asset inventory | Laptop management |
| Incident logs | Downtime tracking |
| Employee onboarding | Access checklist |
| API exports | Ticket analytics |
| Monitoring reports | CPU usage tracking |
| Customer onboarding | Progress tracking |

---

# Spreadsheet Basics

---

# Rows

Horizontal lines.

Example:
```text
1
2
3
4
```

---

# Columns

Vertical sections.

Example:
```text
A
B
C
D
```

---

# Cells

A single box in the spreadsheet.

Example:
```text
A1
B2
C5
```

---

# Example Table

| A | B | C |
|---|---|---|
| Name | Department | Status |
| Alice | Support | Active |
| John | Engineering | Offline |

---

# Why This Matters

Operational systems often export:
- CSV files
- reports
- logs

that engineers analyze in spreadsheets.

---

# Data Types

Spreadsheets can contain:
- text
- numbers
- dates
- percentages
- formulas

---

# Real Support Example

| Ticket ID | Priority | Response Time |
|---|---|---|
| 1001 | High | 5 mins |
| 1002 | Medium | 15 mins |

---

# Formulas

Formulas perform calculations automatically.

All formulas begin with:
```text
=
```

---

# Example

```excel
=A1+B1
```

---

# Important Beginner Formulas

---

# SUM

Adds numbers.

```excel
=SUM(A1:A10)
```

---

# AVERAGE

Calculates average.

```excel
=AVERAGE(B1:B10)
```

---

# COUNT

Counts values.

```excel
=COUNT(C1:C10)
```

---

# MAX

Finds highest value.

```excel
=MAX(A1:A10)
```

---

# MIN

Finds lowest value.

```excel
=MIN(A1:A10)
```

---

# Real Startup Example

Support manager tracks:
- average response time
- number of incidents
- highest downtime duration

using formulas.

---

# IF Statements

Very important for operational logic.

---

# Example

```excel
=IF(B2>90,"Critical","Normal")
```

---

# Real Support Engineering Example

```excel
=IF(C2="Offline","Escalate","Healthy")
```

---

# Conditional Formatting

Automatically changes cell appearance based on conditions.

---

# Example

Highlight:
- high CPU usage
- failed backups
- overdue tickets

---

# Real Startup Usage

Support dashboards often color:
- red → critical
- yellow → warning
- green → healthy

---

# Sorting Data

Sorting organizes information.

---

# Examples

Sort by:
- priority
- ticket age
- response time
- CPU usage

---

# Filtering

Filters display only relevant data.

---

# Example

Show only:
- critical tickets
- offline servers
- overdue onboarding tasks

---

# Why Filters Matter

Support engineers constantly work with large datasets.

Without filtering:
- troubleshooting becomes slow
- reporting becomes difficult

---

# Freeze Panes

Keeps headers visible while scrolling.

Extremely useful for:
- large reports
- incident logs
- inventory sheets

---

# Real Startup Example

An inventory sheet may contain:
- 10,000+ devices

Freezing headers improves navigation.

---

# Data Validation

Controls allowed input.

---

# Example

Only allow:
- High
- Medium
- Low

for ticket priority.

---

# Why Validation Matters

Prevents:
- bad data
- inconsistent formatting
- reporting errors

---

# Common Startup Spreadsheet Systems

---

# IT Asset Inventory

| Device | User | Status |
|---|---|---|
| MacBook Pro | Alice | Assigned |
| Dell XPS | John | Available |

---

# Ticket Tracker

| Ticket ID | Priority | Assigned To |
|---|---|---|
| 2001 | Critical | Tier 2 |
| 2002 | Medium | Tier 1 |

---

# Incident Tracker

| Incident | Duration | Status |
|---|---|---|
| API outage | 15 mins | Resolved |

---

# SLA Monitoring

| Ticket | First Response | SLA Status |
|---|---|---|
| 3001 | 4 mins | Within SLA |

---

# CSV Files

CSV means:
```text
Comma-Separated Values
```

CSV files are heavily used in:
- exports
- APIs
- logs
- monitoring systems

---

# Real Startup Example

Zendesk exports:
```bash
tickets.csv
```

Support engineers analyze it using:
- Excel
- Google Sheets

---

# Importing CSV Files

In Google Sheets:
```text
File → Import
```

In Excel:
```text
Data → From Text/CSV
```

---

# Why CSV Matters

Many APIs export operational data as CSV.

Examples:
- support tickets
- endpoint logs
- monitoring metrics
- onboarding reports

---

# Pivot Tables

Pivot tables summarize large datasets.

---

# Example Questions

- Which engineer resolved the most tickets?
- Which issue category appears most?
- Which department generates most incidents?

---

# Real Startup Example

Support leadership may ask:
> "Which issue category creates the highest support load?"

Pivot tables answer this quickly.

---

# Charts

Spreadsheets can visualize:
- uptime
- ticket trends
- incident spikes
- support KPIs

---

# Common Charts

| Chart | Usage |
|---|---|
| Bar chart | Compare categories |
| Pie chart | Distribution |
| Line chart | Trends over time |

---

# Real Startup Dashboard Example

A support dashboard may show:
- weekly ticket volume
- uptime %
- response times
- incident categories

---

# Spreadsheet Automation Thinking

Modern engineers often combine:
- spreadsheets
- APIs
- Python scripts
- cloud automation

---

# Real Example

A Python script exports:
```bash
server_metrics.csv
```

Google Sheets automatically visualizes:
- CPU usage
- downtime
- alerts

---

# Google Sheets Collaboration

Google Sheets is heavily used because:
- teams collaborate live
- comments are easy
- sharing is fast
- startup teams work remotely

---

# Permission Management

Spreadsheets often contain sensitive data.

Examples:
- employee information
- asset inventory
- operational metrics

---

# Security Best Practices

Never expose:
- passwords
- API keys
- production credentials
- sensitive customer data

inside spreadsheets.

---

# Common Beginner Mistakes

| Mistake | Better Approach |
|---|---|
| Messy formatting | Use clean tables |
| No filters | Add filtering |
| Hardcoded calculations | Use formulas |
| Duplicate data | Normalize structure |
| Poor naming | Use clear headers |

---

# Startup Engineering Best Practices

Professional operational spreadsheets should:
- have clean headers
- use filters
- use validation
- include timestamps
- separate raw data from dashboards
- avoid sensitive secrets

---

# Real Technical Support Workflows

Support engineers commonly use spreadsheets for:
- asset management
- onboarding checklists
- escalation tracking
- SLA reporting
- incident reviews
- API export analysis

---

# Mini Exercises

---

# Exercise 1 — Ticket Tracker

Create a spreadsheet with:

| Ticket ID | Priority | Status |
|---|---|---|

Add:
- 10 sample tickets

---

# Exercise 2 — SLA Formula

Add:
```excel
=IF(C2<15,"Healthy","Late")
```

---

# Exercise 3 — Conditional Formatting

Highlight:
- red for critical
- yellow for warning
- green for healthy

---

# Exercise 4 — Asset Inventory

Create:

| Device | Assigned User | Status |
|---|---|---|

---

# Exercise 5 — Create a Chart

Visualize:
- ticket count by priority

---

# Beginner Project

## Startup Support Dashboard

Build a spreadsheet dashboard showing:
- ticket counts
- SLA performance
- offline systems
- incident trends
- onboarding progress

---

# Real Skills Built Here

This lesson develops:
- operational reporting
- structured thinking
- data organization
- KPI awareness
- analytical thinking

These become valuable in:
- support engineering
- solution engineering
- operations
- customer success
- SaaS support
- startup infrastructure teams

---

# Key Takeaways

- Spreadsheets are operational engineering tools
- Support teams rely heavily on structured reporting
- Formulas automate calculations
- Filters and sorting improve troubleshooting
- CSV files are critical in operational workflows
- Dashboards improve visibility and communication

---

# Next Lesson

Continue to:

```bash
ticketing-systems-basics.md
```

The next lesson explains:
- how real support systems work
- tickets
- SLAs
- escalation
- queues
- incident workflows
- startup support operations
