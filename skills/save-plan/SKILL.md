---
name: save-plan
description: Save a finished learning path by scheduling study sessions in Google Calendar and/or exporting the plan to a Notion page. Use only when the user explicitly asks to schedule, put on the calendar, save, export or send a learning path or review schedule.
---

# Save plan

This skill writes to the user's own accounts, so it needs an explicit request and an explicit confirmation before anything is created.

## Ground rules

- Act only when the user asked to schedule or save. Never do it as a bonus after planning.
- Only create new items. Never edit or delete existing events, pages or databases.
- Read the calendar only inside the time window the user gave, and only to find free slots. Do not summarize, repeat or comment on other events.
- Show a preview and wait for a clear yes before creating anything.
- If a needed connector is not connected, say which one and stop. Offer the plan as plain text to copy instead.
- Do not use stored memory or past chats to fill in preferences. Ask.

## Schedule in Google Calendar

1. Make sure a learning path or review schedule exists in the conversation. If not, offer `/studypath:plan` first.
2. Ask in one message: which days and time windows work, session length (default 45 minutes), start date, and time zone.
3. Check free time inside those windows with the calendar connector and propose sessions, one per plan item, avoiding conflicts.
4. Show a table: date, time, session title, what to do. Ask "Create these events?" and wait.
5. After a yes, create one event per session. Title: `Study: <module> - <lesson or task>`. Put the lesson link, the goal and the checkpoint question in the description. Do not invite other people.
6. Report how many events were created and list any that were skipped because of conflicts.

## Export to Notion

1. Ask where the page should go (a parent page the user names). If they do not know, offer to create it at the top level of their workspace.
2. Show a short preview of the page title and its sections. Wait for a yes.
3. Create one page containing the plan: overview table, modules with lesson links, practice tasks, checkpoints, and a progress checklist. Do not touch any other page.
4. Reply with a one-line confirmation and the page title.

## If something fails

Report the failure plainly, say what was and was not created, and do not retry in a loop. Never repeat a creation that may already have succeeded.
