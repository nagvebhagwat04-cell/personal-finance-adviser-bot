# Personal Finance Adviser Bot
## Project Memory

## 1. Project Identity

**Name:** Personal Finance Adviser Bot  
**Domain:** AI in BFSI  
**Purpose:** Help users understand and plan personal finances using deterministic financial calculations and a Gemini-powered educational assistant.

## 2. Product Boundary

The application is a financial education and planning tool.

It does not:
- Execute financial transactions.
- Connect directly to bank accounts in the MVP.
- Guarantee investment returns.
- Replace regulated professional advice.

## 3. Technology

```text
Frontend: React + Vite + TypeScript
UI: Tailwind CSS
Backend: Node.js + Express + TypeScript
Database: MongoDB + Mongoose
Authentication: JWT + bcrypt
AI: Google Gemini API
Charts: Recharts
Testing: Vitest + Supertest + Playwright
```

## 4. Core Architecture Rule

The backend is the source of truth for financial calculations.

Gemini is responsible for natural-language explanation, education, interpretation, and suggestions based on supplied context.

Gemini must not be treated as the calculation engine.

## 5. Core Modules

- Authentication.
- Financial profile.
- Transactions.
- Budget.
- Financial goals.
- Calculation engine.
- Dashboard.
- AI Adviser.
- Chat history.
- Testing infrastructure.

## 6. Financial Metrics

The application supports:

```text
Monthly surplus
Savings rate
Budget utilization
Emergency-fund requirement
Goal contribution requirement
EMI
Total loan interest
Debt-to-income ratio
```

## 7. Security Memory

```text
GEMINI_API_KEY = backend only
JWT_SECRET = backend only
passwordHash = never returned
userId = derived from authenticated identity
.env = never committed
```

## 8. AI Behavior

The AI should:

- Use supplied financial context.
- Use backend-calculated metrics.
- Explain calculations in plain language.
- State assumptions.
- Ask the user for missing information when needed.
- Avoid inventing financial facts.
- Avoid guaranteed outcomes.
- Provide educational investment explanations.
- Remain transparent about uncertainty.

## 9. Testing Strategy

Testing is a mandatory part of development.

Required layers:

```text
Unit
↓
Component
↓
API Integration
↓
Security
↓
End-to-End
↓
Production Build
↓
Manual QA
```

No feature should be considered complete without appropriate tests.

## 10. Current State

Documentation baseline created.

Implementation status must always be reflected in `TASK.md`.

## 11. Important Decisions

1. Gemini integration occurs only through the backend.
2. Financial calculations are deterministic.
3. MongoDB stores user financial records.
4. JWT protects private APIs.
5. Every user-owned record is scoped to the authenticated user.
6. Testing covers both happy paths and failure paths.
7. AI safety is part of the product requirements, not an optional enhancement.

## 12. Change Log

### v1.0
- Defined product requirements.
- Defined full-stack architecture.
- Defined engineering rules.
- Defined UI/UX requirements.
- Added complete implementation roadmap.
- Added mandatory testing phases.
- Defined persistent project memory.
