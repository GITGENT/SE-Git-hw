# SE-Git-hw
Software Engineering | GIT HW

# Overview
Our class received a hands-on Git & GitHub practice project for CINS 5318 (Software Engineering, Fall 2026, Dr. Mary Kim) | Assignment #1: Version Control using GitHub.

## Project Overview
This repository demonstrates core Git and GitHub workflows: repository setup, committing, branching, pull requests, code review, merge-conflict resolution, and issue tracking.

## Files
| File | Description |
|---|---|
| `hello.py` | "Hello, World!" program with basic error handling — the initial commit, later updated to resolve a merge conflict and close Issue #3. |
| `apple.py` | Prints `I eat apple`, with a docstring added to close Issue #2 — added on the `feature-1` branch. |
| `README.md` | This file. |

## How to Run
```bash
python hello.py
python apple.py
```

## Git Workflow Used
- **Initial commit** — created `hello.py` and pushed to `main`.
- **`feature-1` branch** — added `apple.py`, pushed, opened a pull request, and merged it into `main` after peer review.
- **`conflict-branch`** — created to intentionally edit the same line of `hello.py` as `main`, simulating and then resolving a real merge conflict.

## Pull Requests
- PR #1 — "Add apple.py feature": `feature-1` → `main`, reviewed and merged by jwhawkins68.
- Reviewed James hHawkins JWHAWKINS68 , classmate's PR: [#5 "Conflict branch updates"](https://github.com/Jibus-1/SE-Git-hw/pull/5) on Jibus-1/SE-Git-hw — approved with comments.

## Issues
| # | Title | Assigned to | Status |
|---|---|---|---|
| #2 | Add a Description to Apple.py | GITGENT (self) | Closed |
| #3 | Add Error Handling to Hello.py | jwhawkins68 | Closed |

Both issues were closed automatically via commit messages using GitHub's closing keywords (`closes #2`, `closes #3`).

## Merge Conflict Simulation
A conflict was intentionally created by editing the same line of `hello.py` differently on `main` and `conflict-branch`. Running `git merge conflict-branch` produced `CONFLICT (content): Merge conflict in hello.py`. The conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) were resolved in VS Code by choosing the main branch's version, then committed and pushed with `git commit -m "Resolve merge conflict between main and conflict-branch"`.

## Author
Ryan A. Tucker (GITGENT) | CINS 5318, Fall 2026
