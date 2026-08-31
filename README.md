# Employee Records & Attendance Management System

## Project Overview

This project analyzes employee productivity and operational performance using Microsoft Excel and Power BI.

The objective is to help operations teams monitor task completion, resource utilization, overdue tasks, escalations, and employee performance.

## Business Problem

Operations teams need a simple way to understand:

- How efficiently employees complete assigned tasks
- How effectively working hours are utilized
- Which teams perform better
- Where overdue tasks are increasing
- Which employees may require additional support
- How operational performance changes over time

## Dataset

The project uses simulated operational data for 30 employees over approximately three months.

### Tables

- Employees
- Daily Activity
- Tasks
- DateTable

## Tools Used

- Microsoft Excel
- Power Query
- Power BI
- DAX

## Data Cleaning

The data was cleaned and validated using Power Query.

Key activities included:

- Removing duplicate records
- Standardizing employee information
- Validating dates and numerical values
- Creating calculated fields
- Checking task and productivity data

## Key KPIs

### 1. Task Completion Rate

Measures completed tasks compared with assigned tasks.

### 2. Resource Utilization

Measures productive hours compared with total logged-in hours.

### 3. Overdue Task Rate

Measures the percentage of tasks that were overdue.

### 4. Escalation Rate

Measures escalated tasks compared with completed tasks.

### 5. Tasks Completed

Measures total completed operational tasks.

## Power BI Dashboard

The dashboard contains:

### Executive Summary

- KPI cards
- Weekly task completion trend
- Team performance
- Date filtering
- Team filtering
- Shift filtering

### Team & Employee Drilldown

- Employee performance
- Team comparison
- Productivity analysis
- Utilization analysis

### Trends & Gaps

- Weekly performance trends
- Utilization vs completion analysis
- Top and bottom performers

## DAX

Example:

```DAX
Utilization Measure % =
DIVIDE(
    [Hours Active],
    [Hours Logged In]
)
