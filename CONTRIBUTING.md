# Sending a change

1. **Send it as an issue, with its report.** In a session,
   `/buglog file <id> --with <path>…` writes both: the report, your change as
   a diff per file, and where each file belongs. It opens the **change** form
   filled in; you press Submit. From a shell, `xlii buglog export <id> --with
   <path>…` prints the same to paste into that form.
2. **Say which xlii you ran.** The report carries it: the version, and the
   install (`stock`, `alt` with its sign, or `dev`). A change made against an
   old release is fine; it just needs saying.
3. **Text parts are the easiest:** a card (Markdown), a task (TOML), a seat's
   charter, a doc. Say where each belongs, the same as in xlii
   (`stock_plugins/`, `stock_tasks/`, …).
4. **Code** is welcome the same way, as a diff. The maintainers port it into
   the next release and run the full gate on it. The issue stays the record
   of who made it. A pull request, here or against
   [xlii-computer/xlii](https://github.com/xlii-computer/xlii), is fine too if
   you'd rather send one by hand.
5. **No secrets.** A report or a change that holds a key is deleted.
