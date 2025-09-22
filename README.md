# Generate Senior QA Test

This exercise evaluates how you approach test design, automation, and communication. We expect you to leave the repository runnable so we can execute your tests without manual intervention.

## Scope
Automate Playwright coverage for the Generate Wealth public signup form:
https://www.generatewealth.co.nz/kiwisaver/join/

Focus on the first step of the flow and the *Continue* button validation behaviour. You do not need to test subsequent steps of the form.

## Prerequisites
- Node.js 18+
- npm 9+ (ships with Node 18)
- Chromium/WebKit/Firefox browsers installed via Playwright (`npx playwright install`).

If you lack any of the above, install them before you begin.

## Getting Started
```bash
npm install
npx playwright install
npm test   # describe how to run your suite in package.json or README updates
```
Feel free to replace the placeholder test in `tests/example.spec.ts` with your own structure.

## Core Tasks
1. **Validation coverage** – Trigger *Continue* with each required field empty (individually and collectively) and assert the corresponding error messages. Document the final set of validations you cover.
2. **Happy path smoke** – Provide at least one scenario that fills the form with valid data, clicks *Continue*, and confirms the transition to the next step (or the absence of validation messages).
3. **Accessibility and UX observations** – Note any issues discovered while testing (contrast, focus management, unclear messaging, etc.). Capture them in comments, a markdown file, or your test report.
4. **Reporting** – Produce console output or artifacts (screenshots, traces, HTML report) that demonstrate the results. Mention how to access them in this README if they are not default Playwright outputs.

## Deliverables
- Automated tests located under `tests/` (feel free to reorganise as long as the config still works).
- Any helper utilities or fixtures you deem useful.
- Documentation of assumptions, skipped cases, or flaky behaviour. A `NOTES.md` is fine if it stays lightweight.
- Updates to `package.json` scripts so we can run your suite with a single command (e.g. `npm test`).

## What We Look For
- Clear structure and naming in tests.
- Meaningful assertions that prove validation behaviour.
- Resilience to minor UI timing changes (use locators effectively, avoid brittle selectors).
- Thoughtful comments only where they add clarity.
- Clean git history (optional but appreciated) that reflects your thinking.

## Extras (Optional)
Tackle any of the following if you have time and it adds value:
- Cross-browser execution via Playwright projects or CLI options.
- CI configuration (GitHub Actions, etc.) that runs the suite.
- Visual comparison or screenshot assertions.
- Coverage of edge cases such as international phone numbers or leap-year DOBs.

## How to Submit
Please provide us with a Github (or similar) URL for us to access the code.

**Spend NO MORE THAN 1 HOUR on this task** - don't worry if you don't hit all the requirements perfectly, this is to simply show you have some understanding of automated tests. 

Thanks for taking the time to complete the test, and feel free to show your personality in the approach you take.
