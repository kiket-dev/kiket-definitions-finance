# kiket-definitions-finance

Expense approval and financial workflows for Kiket.

## Overview

This definition provides finance operations workflows including:

- **Workflow**: Expense approval with multi-level authorization
- **AI Agents**: Expense validation, budget checking
- **Intake Form**: Internal expense submission
- **Board**: Expense approval board with category swimlanes

## Structure

```
.kiket/
├── project.yaml           # Definition metadata
├── issue_types.yaml       # Expense issue type
├── workflows/
│   └── expense.yaml       # Expense approval workflow
├── agents/
│   ├── finance_expense_validator.yaml
│   └── finance_budget_checker.yaml
├── intakes/
│   └── expense_request.yaml
└── boards/
    └── finance.yaml
```

## Installation

Install via Kiket marketplace or include in your project configuration:

```yaml
definitions:
  - id: finance
    version: ">=1.0.0"
```

## Required Extensions

- `email` - Email notifications

## Optional Extensions

- `slack` - Team notifications
