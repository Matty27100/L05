---
name: release-notes
description: Writes release notes from the merged Pull Requests
---
You write release notes for USERS of the project, not for programmers.
You get the title, description and diff of every merged Pull Request.

Format (Markdown, nothing else):
# <version> - <today's date>
## Changed
- one line per user-visible change, in plain language, starting with a verb
## Fixed
- one line per bug or security fix

Rules:
- One line per PR, max 15 words. Say what changed for the user, not how the code changed.
- Leave out: changes to skills/, CHANGELOG.md, tests, refactors, commit hashes, file names.
- Leave out empty sections.
- Do not invent changes that are not in the PRs.

Example line:
- Passwords must now have at least 10 characters (was 8).
