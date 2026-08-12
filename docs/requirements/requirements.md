# Leave Management System - Requirements

## 1. Project Overview

The Leave Management System is a Salesforce-based application designed
to manage employee leave requests, leave balances, and company holidays.

The project is being developed step by step while learning Salesforce
development concepts.

The development approach is:

Learn → Build → Test → Document → Deploy

---

## 2. Problem Statement

In a traditional leave management process, employees may submit leave
requests through emails, spreadsheets, or manual forms.

This can lead to:

- Difficulty tracking leave requests
- Manual approval processes
- Incorrect leave balance calculations
- Lack of centralized employee information
- Difficulty maintaining leave history
- Lack of visibility for HR and managers

The Salesforce Leave Management System aims to provide a centralized
platform for managing these activities.

---

## 3. Project Objectives

The main objectives of the system are:

- Store and manage employee information
- Allow employees to submit leave requests
- Validate leave request information
- Maintain employee leave balances
- Manage company holidays
- Support leave approval and rejection
- Automate leave-related processes
- Provide reports and dashboards
- Provide a user-friendly Salesforce interface

---

## 4. Users of the System

### Employee

Employees should be able to:

- View their employee information
- Submit leave requests
- Select a leave type
- Enter leave dates
- Provide a reason for leave
- View their leave request status
- View their available leave balance

### Manager

Managers should be able to:

- View employee information
- View leave requests
- Review leave requests
- Approve leave requests
- Reject leave requests
- Provide comments when required

### HR / Administrator

HR users should be able to:

- Create and manage employee records
- Manage leave balances
- Manage company holidays
- Monitor leave requests
- View reports and dashboards
- Manage Salesforce configuration

---

# 5. Functional Requirements

## 5.1 Employee Management

The system should allow authorized users to:

- Create employee records
- View employee records
- Update employee information
- Maintain employee department and designation
- Maintain employee contact information
- Track employee active status
- Maintain employee leave balance

---

## 5.2 Leave Request Management

The system should allow employees to create leave requests.

A leave request should contain information such as:

- Employee
- Leave Type
- Start Date
- End Date
- Reason
- Applied Date
- Status
- Manager Comments

The system should allow authorized users to view and update
leave request records.

---

## 5.3 Leave Validation

The system should prevent invalid leave requests.

For example:

- End Date should not be earlier than Start Date
- Required information should be provided
- Invalid dates should be prevented
- Rejected requests should follow the required comment rules

Validation Rules will be implemented to enforce these requirements.

---

## 5.4 Leave Approval

The system should support the following process:

```text
Employee
    ↓
Submit Leave Request
    ↓
Pending
    ↓
Manager Reviews
    ↓
 ┌───────────────┐
 ↓               ↓
Approved       Rejected
 ↓               ↓
Update          Store
Balance         Reason/Comment
