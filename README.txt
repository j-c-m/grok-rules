grok-rules
==========

Personal Grok agent rules. Grok loads every *.md in this directory for all
projects (~/.grok/rules/).

Files
-----

  01-coding.md       Coding principles and product-UI/comment rules
  02-language.md     Language: STE for user-facing; jargon OK in tech/chat

Install
-------

  git clone git@github.com:j-c-m/grok-rules.git ~/.grok/rules

If ~/.grok/rules already exists, clone elsewhere and copy or merge the *.md
files into it.

Load order
----------

  1. Home rules: ~/.grok/rules/*.md (this repo), then optional ~/.claude and
     ~/.cursor rules when compatibility is enabled.
  2. Project: from repo root to CWD — AGENTS.md (and aliases: Agents.md,
     AGENT.md, Claude.md, CLAUDE.md, CLAUDE.local.md) plus
     <dir>/.grok/rules/*.md (and optional .claude/.cursor rules dirs).
  3. Deeper project files win when instructions conflict.
  4. Within a rules directory, files load alphabetically.

  See ~/.grok/docs/user-guide/12-project-rules.md.

Notes
-----

  - One rule per line ("- …").
  - No headings inside rule files (saves tokens).
  - This README is plain text so Grok does not load it as a rule.
