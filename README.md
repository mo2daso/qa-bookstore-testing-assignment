# QA Internship Assignments

Repository for QA internship assignments covering manual testing, requirement
analysis, test planning, and test execution using **Testworthy**.

## Project Under Test

All assignments in this repo test the same fictional system: an **Online
Book Store** — an e-commerce platform where users browse, search, and
purchase books, manage their cart, and track orders.

---

## Assignments

### 1. Requirement Analysis
Requirement analysis and documentation for the Online Book Store system,
including:
- Requirement understanding and core workflows
- 12 Functional Requirements (FR-01–FR-12)
- 6 Non-Functional Requirements (NFR-01–NFR-06) — performance, security,
  availability, usability, scalability, reliability
- 11 User Stories (`As a... I want... so that...`)
- 7 Gherkin acceptance criteria scenarios (`Given / When / Then`)

**File:** `Online_Bookstore_Requirement_Analysis.docx`

---

### 2. Test Plan, Test Cases & Execution
Manual testing deliverables built on top of Assignment 1's requirements,
managed and executed in **Testworthy**.

**What's included:**
- A high-level test plan (introduction, scope, objectives, environment,
  testing types, entry/exit criteria, risks & assumptions, deliverables)
- 24 test cases across 5 suites (Authentication, Catalog & Search, Cart,
  Checkout & Orders, Account Management), each classified as Smoke,
  Regression, Negative, or Automation Candidate
- A full test run ("Sprint 1 Regression & Smoke Cycle") executed against
  a staging environment

**Results:** 24 total test cases — **19 Passed, 3 Failed, 2 Blocked**
(79.2% pass rate). Failures and blockers logged with defect references:

| ID | Result | Reason |
|---|---|---|
| TC-007 | Blocked | Test email service not configured in staging |
| TC-014 | Blocked | Out-of-stock handling not yet implemented |
| TC-011 | Failed | Empty search shows a blank page instead of a message |
| TC-019 | Failed | Invalid card shows a generic error, not a specific one |
| TC-023 | Failed | Catalog page load ~3.4s, exceeding the 2s NFR-01 target |

**Files:**
- `Test_Plan_Online_Bookstore.docx` — high-level test plan
- `Test_Cases_Online_Bookstore.csv` — all 24 test cases with steps,
  expected results, priority, type, suite/section, and execution status
- `Test_Run_Report_Online_Bookstore.pdf` — consolidated execution report
- `report-187.pdf`, `report-188.pdf`, `report-189.pdf` — native Testworthy
  exports (Test Plan, Milestone, and Test Run summary reports)

**Tools used:** Testworthy (test case management & execution), Microsoft
Word (test plan), CSV export (test case submission)

---

### 3.

---

## Author

Soban — QA Intern
