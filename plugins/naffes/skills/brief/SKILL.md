---
name: brief
description: The person's day in Naffes CRM — tasks due or overdue, deals closing this week, deals at risk. Use when they ask what to do today, for their briefing, "موجزي اليوم", or "إيه المطلوب مني".
---

# My day in Naffes

Answer in the language the person wrote in.

1. Call `whoami` once if you have not in this conversation. It says whose CRM this is and whether you may change data.
2. Call `my_briefing`. It returns tasks due today or overdue, deals closing this week and the top deals at risk.
3. Write the brief in this order, and leave out a section that is empty:
   - **Overdue** — what is late, oldest first.
   - **Today** — what is due today.
   - **Closing this week** — each deal with its amount and stage.
   - **At risk** — each deal with the one reason it is at risk.
4. End with the single most useful next step, in one sentence.

Rules:
- Every record you name is a link: use the `url` that came with it.
- Use the numbers the tools return. Never count rows yourself and never estimate an amount.
- At most five items per section; say how many more there are.
- Do not change anything. If the person then asks you to complete or move something, confirm the exact record first.
