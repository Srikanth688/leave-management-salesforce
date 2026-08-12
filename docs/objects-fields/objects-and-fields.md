# Objects and Fields

## Overview

Salesforce Objects and Fields form the basic data structure of the
Leave Management System.

## What is an Object?

An Object is used to store a particular type of business data.

It is similar to a table in a database.

Example:

Employee Object → stores employee information.

## What is a Field?

A Field stores one specific piece of information about a record.

Example:

Employee → Email, Department, Designation.

## What is a Record?

A Record is an actual instance of an object.

Example:

Employee Object

Employee Name: Rahul
Department: IT
Designation: Developer

## Simple Database Comparison

Object = Table

Field = Column

Record = Row

---

# Objects Created

The Leave Management System contains four main custom objects.

## 1. Employee

Purpose:

Stores employee information.

Examples of information:

- Employee Name
- Employee ID
- Email
- Phone
- Department
- Designation
- Date of Joining
- Leave Balance
- Active

---

## 2. Leave Request

Purpose:

Stores employee leave applications.

Examples:

- Employee
- Leave Type
- Start Date
- End Date
- Reason
- Status
- Manager Comments

---

## 3. Leave Balance

Purpose:

Stores the leave balance associated with employees.

Examples:

- Employee
- Leave Type
- Available Balance
- Used Leave
- Remaining Leave

---

## 4. Holiday

Purpose:

Stores company holiday information.

Examples:

- Holiday Name
- Holiday Date
- Holiday Type
- Description

---

# Fields

Different Salesforce field types were used according to the
requirements of each object.

Common field types include:

- Text
- Email
- Phone
- Date
- Number
- Picklist
- Checkbox
- Lookup
- Auto Number

---

# Learning

The main concepts learned:

- Salesforce Objects
- Custom Objects
- Salesforce Fields
- Custom Fields
- Field Data Types
- Records
- Object Manager
- Field API Names

---

# Project Status

Status: Completed ✅
