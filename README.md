# Identity & Access Risk Analytics Platform

This project explores a common security and IT-control problem: employees can gradually accumulate permissions that are no longer required for their current roles.

For example, an employee may change departments but continue to retain access from their previous role. Temporary project access may also remain active after the project ends. Over time, this can lead to privilege creep and unnecessary access risk.

To study this problem, I built an end-to-end analytics workflow using synthetic IAM data. The system evaluates employee roles, applications, permissions, and access activity to identify accounts that may require review.

## Data Note

All datasets in this project are synthetically generated for demonstration purposes. They do not contain real employee, permission, or access-log information.

## What the Project Does

The platform identifies:

- Role-mismatched permissions
- Dormant or unused access
- Excessive administrative privileges
- Cross-department access
- After-hours activity
- Unusual login locations
- Failed access attempts
- Unusual access patterns using Isolation Forest

Each employee receives an explainable risk score and risk category. The dashboard also shows the main reasons behind the risk classification.

## Dashboard

The Power BI dashboard includes three pages:

### Executive Overview

- Total employees and permissions
- Risky and high-risk account metrics
- High-risk employee table
- Employee-level drill-through

### Risk Analytics

- High-risk accounts by department
- Risk-level distribution
- Dormant permissions by department

### Employee Investigation

- Employee risk summary
- Assigned applications and permissions
- Recent access activity
- Risk reasons and access details

  ## Interactive Demo

[Watch the dashboard walkthrough](demo/dashboard_demo.mp4)


## Project Workflow

```text
Synthetic IAM data
        ↓
Data preparation and analysis
        ↓
Rule-based risk scoring
        ↓
Isolation Forest anomaly detection
        ↓
Power BI dashboard
```

## Usage

This repository is shared for portfolio and evaluation purposes.
Please contact me before reusing or redistributing the code or project materials.


