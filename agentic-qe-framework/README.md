# Agentic QE Framework — Demo Video

A proof-of-concept **multi-agent quality engineering pipeline** that takes a Jira story to a verified release autonomously.

📹 **[agentic-qe-framework-demo.mp4](agentic-qe-framework-demo.mp4)** — 2¼-minute recorded walkthrough of the full pipeline (1280×720).

## The POC

Five specialised agents hand off to each other, end to end:

| # | Agent | Responsibility |
|---|-------|----------------|
| 1 | **Reader** | Ingests the Jira story and extracts test intent from the acceptance criteria |
| 2 | **Generator** | Writes the Playwright test spec (e.g. `cart.spec.ts`) from the extracted intent |
| 3 | **Runner** | Executes the spec against the application under test, step by step |
| 4 | **Healer** | Triggered on failure — inspects the DOM, repairs broken locators, and re-runs until the test passes clean |
| 5 | **Reporter** | Files the defect with severity, reproduction steps, and run artifacts (logs + screenshots), linked back to the originating story |

## What the demo shows

The recording follows a single story (`QE-482 — Cart subtotal should equal item price for a single item`) through the whole pipeline:

1. Reader parses the story and its acceptance criteria into test intent.
2. Generator produces the Playwright spec.
3. Runner executes it against a demo shop application.
4. A locator failure (`#subtotal-label not found`) escalates to the Healer, which repairs the selector; the healed test runs clean on attempt 2.
5. Reporter files defect `QE-491`, linked to `QE-482`, with steps to reproduce and run artifacts attached.

## Why it matters

The POC demonstrates where agentic automation genuinely removes QE toil:

- **Intent extraction** — no manual translation from acceptance criteria to test cases
- **Self-healing selectors** — flaky-locator maintenance handled inside the pipeline
- **Evidence-backed defect creation** — defects arrive pre-linked to the story with logs and screenshots attached

## Source code

The implementation is a **private proof of concept** — the source is not published in this repository. Only the recorded demo is shared here.

## Tech

`Agentic AI` · `Multi-Agent Pipeline` · `Playwright` · `Self-Healing Tests` · `Jira Integration` · `QE Automation`
