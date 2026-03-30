---
name: debug
description: Use when the user says "debug", "fix", "doesn't work", "error", "something is broken", "not working", "getting an error", or describes a bug in their web app. Diagnoses and fixes issues in Flask + HTML/CSS + SQLite projects.
---

# Debug

Find, fix, and explain problems in web application code.

## Problem Categories

- **Route issues** — Flask routes not working, 404 errors, Blueprint connection problems
- **Template issues** — Missing variables, Jinja2 rendering failures, template inheritance errors
- **Database issues** — SQLAlchemy errors, connection failures, migration problems
- **Auth issues** — Login not working, password validation failing, session problems
- **Frontend issues** — JS not executing, CSS not applying, form submission failures

## Diagnostic Process

1. Check logs and read relevant files to diagnose the issue automatically
2. If the cause is not clear from logs, run the app and attempt to reproduce the problem
3. Report findings to the user

## Fix Process

1. Explain why the error happened and describe the planned fix
2. Wait for user permission before making changes
3. Implement the fix
4. Explain what was changed and why
5. Verify the fix by running the app again
