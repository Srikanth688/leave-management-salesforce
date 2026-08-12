# Salesforce Object Relationships

## Overview

Relationships connect records between Salesforce objects.

They allow related business information to be accessed together.

---

# Why Relationships Are Needed

Without relationships:

Employee information

and

Leave Request information

would exist separately.

With relationships:

Employee
   ↓
Leave Requests

Salesforce can understand which leave requests belong to which employee.

---

# Relationships in the Project

## Employee → Leave Request

An employee can have multiple leave requests.

Example:

Employee: Rahul

- Leave Request 001
- Leave Request 002
- Leave Request 003

Conceptually:

Employee
   |
   | 1
   |
   |------< Many
             |
             Leave Requests

---

## Employee → Leave Balance

An employee is associated with their leave balance.

Employee
   ↓
Leave Balance

---

# Related List

The Employee record can display related Leave Requests.

Example:

Employee: Rahul

Related List:

Leave Requests

- LR-001
- LR-002
- LR-003

---

# Learning

Concepts learned:

- Object relationships
- Lookup relationships
- Parent and child concepts
- Related Lists
- Relationship fields
- Record connections

---

# Project Status

Status: Completed ✅
