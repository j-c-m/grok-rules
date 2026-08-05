grok-rules
==========

Personal Grok agent rules. Grok loads every *.md in this directory for all
projects (~/.grok/rules/).

Files
-----

  01-coding.md       Coding principles and UI/comment rules
  05-asd-ste100.md   Prefer STE100; soft, not full lock-in





Install
-------

  git clone git@github.com:j-c-m/grok-rules.git ~/.grok/rules

If ~/.grok/rules already exists, clone elsewhere and copy or merge the *.md
files into it.

Notes
-----

  - One rule per line ("- …").
  - No headings inside rule files (saves tokens).
  - This README is plain text so Grok does not load it as a rule.
  - Project rules in <repo>/.grok/rules/ still apply.
