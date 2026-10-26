# xlii reports

The official place to report what xlii got wrong, ask for what it should do,
and send changes back: issues and pull requests, from any version of xlii,
stock or changed.

xlii itself lives at [xlii-computer/xlii](https://github.com/xlii-computer/xlii)
(`pip install xlii`). This repo is kept apart on purpose: reports arrive from
every release people run, and from installs they have changed, not only the
latest one.

## The fastest report is the one xlii writes

In a session, `/buglog` files what just happened, with the tape and the logs
as layers. Then:

    /buglog file b12

shows you the exact report: what happened, xlii's version, and whether the
install is stock or changed (`stock` · `alt` with its sign · `dev`). Secrets
are redacted, and the report says how many spans it took out. On your yes it
opens this repo's new-issue page with that report filled in, and you press
Submit under your own GitHub account. xlii sends nothing by itself.

`/buglog file` arrives with the next xlii release. Until then, and from any
shell, `xlii buglog export b12` prints the same report to paste here.

## What a report carries

- **The version** (`xlii --version`, e.g. `0.26276.7050`).
- **The divergence stamp:**
  - `stock`: every file is as pip installed it.
  - `alt`: files were changed, added or removed, with a short hash and the
    sign derived from it, so the same change always reads the same.
  - `dev`: a source checkout.
  - `unknown`: nothing to compare against.
- **Where it happened, and the home brain.**
- **The buglog row:** what was said and done, and the evidence xlii kept.

## Pull requests

Welcome, especially for the plain-text parts of xlii that anyone can shape:

- cards (a plugin is a Markdown file);
- tasks (TOML);
- seats and their charters;
- docs.

A code change against a release is ported into the lab by the maintainers and
ships with the next release; the pull request stays the record of who made it.

Be specific, be kind, and leave secrets out. A report that holds an API key is
deleted.
