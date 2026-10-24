# PaperTrail

An offline-first resume and CV studio with version history, application tracking, reminders, and recruiter-ready exports. PaperTrail runs entirely in the browser from a single HTML file - no account, server, or data upload is required.

## Highlights

- Build separate resume and academic CV documents.
- Choose from Classic, Modern, Compact, and Split Column ATS-safe templates.
- Control font family, accent colour, type size, margins, line height, section gaps, and item gaps.
- Preview content as paginated A4 pages, a continuous document, or plain ATS text.
- Save named versions for each target company with tags and notes.
- Export the current document or any saved version as PDF, DOCX, or TXT.
- Track applications, statuses, follow-up dates, next steps, and linked document versions.
- Add per-application reminders with advance notice, repeat behaviour, and toast control.
- Back up or restore the complete workspace as JSON.
- Follow the built-in 10-step tour for document design, exports, backup/import, notifications, and toast settings.

## Getting started

1. Download or clone this repository.
2. Open `PaperTrail_Resume_Studio_fixed.html` in a modern desktop browser.
3. Replace the sample information with your own details.
4. Use **Save version** before tailoring or applying to a role.
5. Export a PDF or DOCX, then log the application in **Tracker**.

No package install, build step, or web server is needed.

## PDF export

PaperTrail offers two PDF modes in **Settings → Export & download flow**:

| Mode | Best for | Behaviour |
| --- | --- | --- |
| Direct download | Fast application uploads | Creates an immediate, selectable-text PDF. It uses portable PDF serif/sans faces and balances short final sections to avoid nearly blank trailing pages. |
| Print dialog | Exact browser typography | Opens an A4-locked print sheet after browser and web fonts are ready. In the browser print dialog, select **Save as PDF** and keep the scale at **100%**. |

Use the Print dialog when the exact installed or web-font appearance is important. Use Direct download when you want a quick, compact, selectable-text file without a save dialog.

## Data and privacy

All workspace data is stored in your browser's local storage. It is not sent to a server.

- Select **Backup JSON** regularly, especially before clearing browser data or moving to another device.
- Select **Import JSON** to restore documents, versions, applications, reminders, and notification settings.
- Import replaces the current workspace after confirmation.

## Notifications and reminders

The notification bell shows due follow-ups and reminders whose advance window has begun. In **Settings → Notifications**, choose whether bell toasts are enabled and how often they repeat. Each application also has its own Notifier settings for reminder date/time, advance notice, repeat behaviour, and toast permission.

## Keyboard shortcuts

| Shortcut | Action |
| --- | --- |
| `Ctrl/Cmd + S` | Save a version |
| `Ctrl/Cmd + P` | Export the current document as PDF |
| `Esc` | Close an open modal, end the tour, or exit fullscreen preview |

## Browser support

Use a current Chromium-based browser, Firefox, or Safari. For the most consistent PDF typography, use a current desktop Chromium browser and the Print dialog PDF mode.
