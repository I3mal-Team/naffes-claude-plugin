---
name: pipeline-review
description: Review the sales pipeline in Naffes CRM — totals by stage, stuck and at-risk deals, and what to do about each. Use for a weekly pipeline review, a forecast check, "راجع البايبلاين", or "إيه وضع الصفقات".
argument-hint: "[pipeline or owner name, optional]"
---

# Pipeline review

Answer in the language the person wrote in. $ARGUMENTS narrows the review to one pipeline or one owner when given.

1. `whoami` once, if not already called.
2. `pipeline_health` for the shape of the pipeline, then `deal_stats` for the totals.
3. `at_risk_deals` for the deals that need attention.
4. For the three largest at-risk deals, call `get_history` on each to see the last real contact — a note, a call, a message.

Write:
- **The numbers** — open deals, total value, and value per stage, as a small table.
- **What is stuck** — deals with no activity, longest silence first, with the date of the last contact.
- **What is at risk** — each deal, why, and one concrete next step (who to call, what to send).
- **One line on the forecast** — what is realistically closing this month.

Rules:
- Every deal you name is a link: use its `url`.
- Totals come from the tools (`total`, the stats). Never add up the rows you were shown.
- If a tool says an object or report is not available to this person, say so plainly and carry on with the rest.
- This is a read. Do not move a stage or edit a deal unless the person asks, and then confirm the deal and the change first.
