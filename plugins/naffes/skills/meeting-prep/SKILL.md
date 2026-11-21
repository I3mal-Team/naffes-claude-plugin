---
name: meeting-prep
description: Prepare for a meeting or call with a customer from Naffes CRM — who they are, open deals, what was last said, what is still owed. Use when the person names a contact or company and asks to prepare, for a summary of an account, or "جهزني لاجتماع مع".
argument-hint: "<contact or company name>"
---

# Meeting prep

Answer in the language the person wrote in. The customer is: $ARGUMENTS

1. `search` for the name. If more than one record matches, list them with their links and ask which one — never guess.
2. `fetch` the record. For a contact, also fetch their company; for a company, `find_records` for its open deals.
3. `get_history` on the contact or deal: notes, calls, tasks, emails and the latest messages.

Write one page:
- **Who** — name, role, company, how long they have been a customer, the owner on our side.
- **Open business** — each open deal with stage, amount and expected close.
- **Last contact** — when, by whom, and what was said, in two or three lines. Quote a request or a promise exactly.
- **Still owed** — open tasks and anything we said we would do and have not.
- **Three things to raise** — grounded in the history above, not generic advice.

Rules:
- Every record you name is a link: use its `url`.
- Say "no record of that" when the history does not show something. Do not fill gaps with what is usual.
- This is a read. Log a note or create a follow-up task only if the person asks.
