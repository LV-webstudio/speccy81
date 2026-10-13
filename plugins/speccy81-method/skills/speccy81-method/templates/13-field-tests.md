# Field tests · <project> · <date>

## 1. Setup (check BEFORE starting)
| What | Value | Checked? |
|---|---|---|
| Machines and devices (model, OS, app version) | | |
| How each piece is started (**from a clean terminal**, not from another session or process that inherits variables) | | |
| Permission mode / configuration of each session (e.g. no automatic mode if approvals are being tested) | | |
| Settings the test needs switched on (e.g. push notifications, Remote Control, USB debugging) | | |
| Test data (real or seed; never personal data in screenshots that get saved) | | |
| Who executes and who observes (user / session / another machine) | | |
| How it is observed (screenshots, ADB, logs, `dumpsys`, console) | | |
| **«It builds» gate:** type check and production build green on the commit being tested (the dev server does not guarantee it) | | |

## 2. Tests
| # | Test | What it confirms | Steps | Expected result | Priority |
|---|---|---|---|---|---|
| P1 | | | | | High |

## 3. Results
| # | Result (✅ / ❌ / ⚠ not valid) | Time | Evidence (screenshot, output) | Detail |
|---|---|---|---|---|
| P1 | | | | |

«⚠ not valid» = the setup did not meet table 1; it is repeated and does not count as a product failure.

**A failing test is not skipped:** it is repeated (e.g. 3 times) to tell flaky from real, the capture is checked and the cause is found: the test or the app. If it is finally skipped, it is recorded as «skipped» with the reason.

## 4. Findings and changes
| Finding | Affects (rule / document / code) | Change made at the same time |
|---|---|---|
| | | |

## 5. Pending to repeat
-
