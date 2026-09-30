---
name: avoid-overengineering
description: Use for coding, fixes, reviews and test changes. Keep work focused on the user's request; avoid unnecessary features, checks, dependencies and tests.
---

# Avoid overengineering

Make the smallest complete, readable change that meets the user's request. Apply these rules while working; do not create extra user checklists or approval steps.

- Establish which responsibilities belong to the tool and which remain manual or external. Add support only where the requested behavior requires it.
- Complete the requested outcome across all necessary files. Ask only when missing information materially changes the task or the permission needed.
- Give every addition a clear reason: requested behavior, an existing requirement, or a repeatable bug within that responsibility. Leave it out if you cannot name the need.
- Read the relevant code and reuse existing flows, checks, built-in features and libraries. Add helpers, files, dependencies or configuration only when the current task needs them. Keep required safeguards without adding duplicate checks.
- Before adding a blocking check or confirmation step, identify the real problem it prevents and the work it stops. Money, imagined misuse or possible future needs alone do not justify it.
- Review the task's scope and your assumptions before chasing unusual cases. Report only plausible failures that break actual requirements; leave correct code unchanged.
- Before extending broken code, check whether the feature is needed. Remove unnecessary code and the data handling, checks, tests and documentation added only to support it.
- Test required behavior and meaningful failure cases. Passing tests show behavior, not whether a feature is needed. Avoid tests that simply repeat the code's logic or check that a removed feature is absent.
- Run required checks and keep testing proportionate to the change. Repeat broad test runs only after relevant changes, failures or unresolved concerns. Consider maintenance, new failure risks, running time, processing cost and user effort; stop when the requested behavior is complete and checked.
