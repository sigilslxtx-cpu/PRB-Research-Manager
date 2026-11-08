# PRB-Research-Manager

## Open a task from a link

This app accepts **review-only To-Do task links**. A link opens the existing To-Do view and a prefilled task editor; it does not create a task until the user chooses **Create record**. After saving, the app selects the matching To-Do category (Today, Upcoming, Unscheduled, etc.). The To-Do and Tasks screens use the same task records.

Example URL (requires this app to be published on GitHub Pages):

`https://sigilslxtx-cpu.github.io/PRB-Research-Manager/#add-task?title=Review%20genealogy%20courses&dueDate=2026-11-15&priority=High`

The link uses a URL **fragment**, so the task fields are not included in the page request to GitHub Pages. Supported fields: `title` (required), `description`, `notes`, `priority` (High/Medium/Low), `status` (Not started/In progress/Waiting on response/Blocked/Deferred/Completed/Cancelled), `dueDate`, `dueTime`, `followupDate`, `assignedTo`, `contact`, and optional existing `projectId`. Percent-encode all field values.

**Safety:** Links are not secure messages. Do not put private client records, passwords, or sensitive casework details in links. No task is saved automatically. The app checks for likely duplicates, requires user review, and confirms browser storage after a link-based save. The browser’s local data store must be accessible. A different browser, device, or app origin will have a different task store. Back up your workspace regularly.

The source is hosted publicly on GitHub; this URL feature does not add logins, cloud synchronization, or source-code privacy.
