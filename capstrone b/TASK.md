# Personal Finance Adviser Bot
## Implementation and Testing Task Plan

## Status Legend

- [ ] Not started
- [~] In progress
- [x] Completed
- [!] Blocked

## Phase 1 – Project Setup

- [ ] Initialize repository.
- [ ] Create frontend with React + Vite + TypeScript.
- [ ] Create backend with Node.js + Express + TypeScript.
- [ ] Configure Tailwind CSS.
- [ ] Configure ESLint and formatting.
- [ ] Create `.env.example`.
- [ ] Create project scripts.
- [ ] Verify frontend starts.
- [ ] Verify backend starts.

## Phase 2 – Database

- [ ] Configure MongoDB connection.
- [ ] Create User model.
- [ ] Create Transaction model.
- [ ] Create Budget model.
- [ ] Create Goal model.
- [ ] Create ChatMessage model.
- [ ] Add indexes.
- [ ] Test database connection.

## Phase 3 – Authentication

- [ ] Create registration endpoint.
- [ ] Hash passwords.
- [ ] Create login endpoint.
- [ ] Generate JWT.
- [ ] Create authentication middleware.
- [ ] Protect private routes.
- [ ] Create frontend login page.
- [ ] Create frontend registration page.
- [ ] Test invalid credentials.
- [ ] Test unauthorized requests.

## Phase 4 – Financial Profile

- [ ] Create profile API.
- [ ] Create profile form.
- [ ] Add validation.
- [ ] Connect frontend to API.
- [ ] Test profile retrieval and update.

## Phase 5 – Transactions

- [ ] Create transaction schema.
- [ ] Create transaction CRUD APIs.
- [ ] Create transaction form.
- [ ] Create transaction list.
- [ ] Add filtering.
- [ ] Add edit.
- [ ] Add delete.
- [ ] Test transaction ownership.

## Phase 6 – Budget

- [ ] Create budget model/API.
- [ ] Create budget UI.
- [ ] Calculate category utilization.
- [ ] Calculate total utilization.
- [ ] Add budget dashboard cards.
- [ ] Test budget calculations.

## Phase 7 – Financial Goals

- [ ] Create goal model/API.
- [ ] Create goal form.
- [ ] Create goal cards.
- [ ] Calculate goal progress.
- [ ] Calculate required monthly contribution.
- [ ] Handle expired deadlines.
- [ ] Test goal calculations.

## Phase 8 – Financial Calculation Engine

- [ ] Implement monthly surplus.
- [ ] Implement savings rate.
- [ ] Implement emergency-fund requirement.
- [ ] Implement EMI.
- [ ] Implement total loan interest.
- [ ] Implement debt-to-income ratio.
- [ ] Implement goal contribution.
- [ ] Add input validation.
- [ ] Add unit tests for normal values.
- [ ] Add unit tests for zero values.
- [ ] Add unit tests for boundary values.
- [ ] Add unit tests for invalid values.

## Phase 9 – Dashboard

- [ ] Create dashboard layout.
- [ ] Create metric cards.
- [ ] Create income/expense chart.
- [ ] Create budget visualization.
- [ ] Create goal visualization.
- [ ] Create recent transactions.
- [ ] Add AI financial summary.
- [ ] Connect all data to backend.
- [ ] Test loading/empty/error states.

## Phase 10 – Gemini AI Integration

- [ ] Configure Gemini SDK.
- [ ] Create backend Gemini service.
- [ ] Create system prompt.
- [ ] Create financial context builder.
- [ ] Add deterministic metrics to AI context.
- [ ] Create `/api/ai/chat`.
- [ ] Create chat history endpoint.
- [ ] Save messages.
- [ ] Build AI chat frontend.
- [ ] Add suggested prompts.
- [ ] Add loading state.
- [ ] Add AI error state.
- [ ] Test Gemini API failure.
- [ ] Test missing API key.
- [ ] Verify API key is never sent to frontend.

## Phase 11 – Security Testing

- [ ] Test password hashing.
- [ ] Test JWT validation.
- [ ] Test expired token.
- [ ] Test invalid token.
- [ ] Test protected routes.
- [ ] Test user-data isolation.
- [ ] Test IDOR-style access attempts.
- [ ] Test invalid request payloads.
- [ ] Test oversized/unexpected input.
- [ ] Check `.env` is ignored by Git.
- [ ] Verify no secret exists in frontend bundle.

## Phase 12 – Frontend Testing

- [ ] Test login form.
- [ ] Test registration form.
- [ ] Test profile form.
- [ ] Test transaction form.
- [ ] Test budget form.
- [ ] Test goal form.
- [ ] Test calculator forms.
- [ ] Test AI chat.
- [ ] Test error states.
- [ ] Test responsive layouts.

## Phase 13 – API Integration Testing

- [ ] Test registration success.
- [ ] Test duplicate email.
- [ ] Test login success.
- [ ] Test invalid login.
- [ ] Test protected endpoint without JWT.
- [ ] Test transaction CRUD.
- [ ] Test budget creation.
- [ ] Test goal CRUD.
- [ ] Test dashboard response.
- [ ] Test EMI calculation endpoint.
- [ ] Test goal calculation endpoint.
- [ ] Test AI chat endpoint.
- [ ] Test chat history authorization.

## Phase 14 – End-to-End Testing

Primary flow:

```text
Register
→ Login
→ Complete Profile
→ Add Income
→ Add Expenses
→ Create Budget
→ Create Goal
→ Open Dashboard
→ Verify Calculations
→ Open AI Adviser
→ Ask Financial Question
→ Receive AI Response
→ Refresh
→ Verify Chat History
```

Additional flows:

- [ ] User can log out.
- [ ] User cannot access another user's data.
- [ ] Invalid forms show useful errors.
- [ ] Empty dashboard works.
- [ ] Gemini failure displays a recoverable error.
- [ ] Mobile layout works.
- [ ] Browser refresh preserves authenticated state correctly.

## Phase 15 – Performance and Reliability Testing

- [ ] Test dashboard with realistic transaction volume.
- [ ] Test repeated API requests.
- [ ] Test database connection failure.
- [ ] Test Gemini timeout/failure.
- [ ] Verify loading states.
- [ ] Verify no unhandled promise rejections.
- [ ] Verify no console errors in normal use.

## Phase 16 – Demo Data

- [ ] Create seed script.
- [ ] Add sample user.
- [ ] Add sample income.
- [ ] Add sample expenses.
- [ ] Add sample budget.
- [ ] Add sample goals.
- [ ] Add sample chat history.
- [ ] Verify dashboard is populated.

## Phase 17 – Documentation

- [ ] Complete PRD.md.
- [ ] Complete ARCHITECTURE.md.
- [ ] Complete RULES.md.
- [ ] Complete DESIGN.md.
- [ ] Keep TASK.md updated.
- [ ] Complete MEMORY.md.
- [ ] Create README.md.
- [ ] Document environment variables.
- [ ] Document local setup.
- [ ] Document testing commands.
- [ ] Document Gemini setup.

## Phase 18 – Production Readiness

- [ ] Run frontend lint.
- [ ] Run backend lint.
- [ ] Run unit tests.
- [ ] Run integration tests.
- [ ] Run end-to-end tests.
- [ ] Run production frontend build.
- [ ] Run production backend build.
- [ ] Verify environment variables.
- [ ] Remove debug logs.
- [ ] Review security.
- [ ] Review accessibility.
- [ ] Review responsive design.
- [ ] Perform final manual QA.

## Definition of Done

A feature is complete only when:

1. Its frontend behavior works.
2. Its backend API works.
3. Its database behavior works where applicable.
4. Validation exists.
5. Error handling exists.
6. Relevant automated tests pass.
7. Security/authorization is verified.
8. Documentation is updated.
9. The feature works in a production build.

## Required Test Commands

Use the project's actual package scripts, with the target structure equivalent to:

```text
npm run lint
npm run test
npm run test:integration
npm run test:e2e
npm run build
```

Do not mark a test phase complete merely because the application starts.
