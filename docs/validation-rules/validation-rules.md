# Salesforce Validation Rules

## Overview

Validation Rules prevent users from saving invalid data.

A Validation Rule contains:

1. Error Condition Formula
2. Error Message

---

# Important Concept

If the formula evaluates to TRUE:

❌ Salesforce displays an error and prevents the record from being saved.

If the formula evaluates to FALSE:

✅ Salesforce allows the record to be saved.

---

# Validation Rule 1

## End Date Cannot Be Before Start Date

### Requirement

An employee cannot submit a leave request where the End Date
is earlier than the Start Date.

### Logic

End Date < Start Date

### Example

Start Date = 20-Aug-2026

End Date = 18-Aug-2026

The condition becomes:

18 < 20

Result:

TRUE

Therefore Salesforce blocks the record.

### Error Message

End Date cannot be earlier than Start Date.

---

# Testing

## Test Case 1 - Invalid

Start Date:

20-Aug-2026

End Date:

18-Aug-2026

Expected:

Error should be displayed.

Actual:

Salesforce prevented the record from being saved.

Result:

PASS ✅

---

## Test Case 2 - Valid

Start Date:

20-Aug-2026

End Date:

22-Aug-2026

Expected:

Record should save.

Result:

PASS ✅

---

# Planned Validation Rules

The following rules will be added during development:

- End Date cannot be before Start Date
- Reason should be provided
- Start Date validation
- Manager Comments required when request is rejected

---

# Learning

Concepts learned:

- Validation Rules
- Formula expressions
- Comparison operators
- TRUE and FALSE evaluation
- Error Messages
- Validation testing

---

# Project Status

Validation Rule 1: Completed ✅

Remaining Validation Rules: In Progress 🔨
