# SauceDemo QA Portfolio

Manual QA project on **Swag Labs (SauceDemo)**, a public demo e-commerce app: test plan, requirements, test cases, execution results and bug reports, with automation planned next.

> SauceDemo (https://www.saucedemo.com) is a practice site by Sauce Labs. This project is independent and not affiliated with Sauce Labs.

## Project Overview

| | |
|---|---|
| **Application under test** | Swag Labs web app, https://www.saucedemo.com |
| **Testing type** | Manual functional testing (positive, negative, boundary, exploratory) |
| **Environment** | Chrome 154 on Ubuntu 24.04 LTS |
| **Author** | HILARY SAMSON |

## What's in This Repository

| Deliverable | Description | Location |
|---|---|---|
| Test Plan | Scope, approach, environment, risks, entry and exit criteria | [Docs](Docs/) |
| Requirements (mini FRS) | 27 requirements (FR-1.1 to FR-7.2) derived from observing the app | [Docs](Docs/) |
| Test Cases | 47 cases traced to requirements, with priority, type and results | [Docs](Docs/) |
| Bug Report | Defect log with severity, priority, steps and evidence | [Bug report (CSV)](Docs/Bug_Report_Refined%20for%20github.csv) |
| Defects | Each bug filed as a GitHub Issue | [Issues](../../issues) |

## Scope

**Tested:** Login, Products page, Product details, Sort dropdown, Cart, Cart page, Checkout, Logout, Reset App State.

**Not in scope:** performance and load testing, penetration testing, accessibility, mobile and responsive layouts, localisation, visual design, external links.

## Approach

- Every test case traces to a requirement ID, and every requirement has at least one test case.
- Cases are prioritised (High, Medium, Low) and run High first.
- Test design uses equivalence partitioning, boundary value analysis and error guessing.
- Every failed case is reported as a GitHub Issue with environment, steps, expected result, actual result and screenshots.

## Results at a Glance

| Metric | Result |
|---|---|
| Test cases executed | 47 |
| Passed | 45 |
| Failed | 2 |
| Defects raised | 2 |

| Bug | Title | Severity | Status |
|---|---|---|---|
| [#1](../../issues/1) | Checkout proceeds with an empty cart | Medium | Open |
| [#2](../../issues/2) | Product buttons still show "Remove" after Reset App State until the page is refreshed | Low | Open |

## Skills Demonstrated

- Test planning and requirements analysis
- Test case design (positive, negative, boundary) with requirement traceability
- Manual test execution and results tracking
- Defect reporting with severity and priority, using GitHub Issues
- Basic test documentation and reporting

## Roadmap

- [x] Test plan, requirements and test cases
- [x] Manual execution and defect reporting
- [ ] Test summary report
- [ ] UI test automation with Playwright (TypeScript)
- [ ] API testing with Postman and Playwright
- [ ] CI pipeline with GitHub Actions, so tests gate every pull request
