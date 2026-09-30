---
name: avoid-overengineering
description: Use for coding, fixes, reviews and test changes. Prefer short, complete solutions; avoid unnecessary features, blocking checks, dependencies and tests.
---

# Avoid overengineering

Make the shortest complete change that meets the user's request. Prefer shorter code even when a longer version would be easier for a human to read. Correctness and requested behavior take priority. Do not create extra user checklists or approval steps.

- Establish which responsibilities belong to the tool and which remain manual or external. Add support only where the requested behavior requires it.
- Complete the requested outcome across all necessary files. Ask only when missing information materially changes the task or the permission needed.
- Justify additions by requested behavior, existing requirements or repeatable bugs. Remove unnecessary features and their supporting code, data handling, checks, tests and documentation rather than extending them.
- Trace the affected flow and relevant callers before editing. Fix the cause where it belongs so all affected callers receive the fix.
- Prefer existing code, then the standard library, native platform features, installed libraries, and finally custom code. Use the first option that meets the requirements; keep the search brief.
- Prefer deletion and the smallest complete diff. Add helpers, files, dependencies, abstractions or configuration only for current requirements; omit scaffolding for hypothetical future work.
- Before adding a blocking check or confirmation step, identify the actual failure it prevents and the work it stops. Money, hypothetical misuse or future needs alone do not justify it.
- Preserve required boundary validation, security, protection against data loss and accessibility. Do not add duplicate safeguards.
- Review scope and assumptions before unusual cases. Flag concrete failures that break actual requirements; leave correct code unchanged. Between equally short options, choose the one that handles relevant edge cases.
- Briefly note deliberate limits when they affect real use. Retain tuning that actual variability requires, such as hardware calibration.
- Use existing tests and the smallest checks that prove changed behavior and meaningful failures. Passing tests show behavior, not necessity. Avoid tests that mirror code or merely check that a removed feature is absent.
- Run required checks; repeat broad tests only for relevant changes, failures or unresolved concerns. Consider maintenance, failure risk, runtime, processing cost and user effort. Stop when the complete outcome is checked.
- Keep progress and explanations concise without fixed length caps. Give the detail the user requests.
