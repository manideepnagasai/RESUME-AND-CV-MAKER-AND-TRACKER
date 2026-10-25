<div align="center">

# 📄 PaperTrail

**Resume & CV Studio · Versioned Snapshots · JD Tailoring · Application Tracker · Reminders**
One offline HTML file. No server. No account. No build step.

[![single-file](https://img.shields.io/badge/build-single%20HTML%20file-0c6b58?style=for-the-badge)](#)
[![offline](https://img.shields.io/badge/works-100%25%20offline-b45309?style=for-the-badge)](#)
[![deps](https://img.shields.io/badge/dependencies-zero-2456c4?style=for-the-badge)](#)


*Build an ATS-safe resume and an academic CV, preview exact A4 pages, tailor with JD keyword match, audit with Resume Health, snapshot versions per company, track every application with reminders — and export PDF / DOCX / TXT / JSON / ZIP in your saved style.*

</div>

---

## 📑 Table of Contents

- [Why PaperTrail](#-why-papertrail)
- [Quick Start](#-quick-start)
- [First-Run Flow (recommended)](#-first-run-flow-recommended)
- [Feature Guide](#-feature-guide)
  - [Build & Preview](#build--preview)
  - [Design & Format](#design--format)
  - [JD Keyword Match](#jd-keyword-match)
  - [Resume Health](#resume-health)
  - [Versions & Snapshots](#versions--snapshots)
  - [Exports & Bundles](#exports--bundles)
  - [Application Tracker + Notifier](#application-tracker--notifier)
  - [Bell Notifications](#bell-notifications)
  - [Settings, Backups & Safety Copies](#settings-backups--safety-copies)
  - [Help, Guided Tour & Field Guide](#help-guided-tour--field-guide)
  - [Mobile Layout](#mobile-layout)
  - [Fullscreen Studio](#fullscreen-studio)
- [File Formats & Schemas](#-file-formats--schemas)
- [Data & Privacy](#-data--privacy)
- [Keyboard Shortcuts](#-keyboard-shortcuts)
- [Under the Hood](#-under-the-hood)
- [ATS Cheat Sheet](#-ats-cheat-sheet)
- [Roadmap](#-roadmap)
- [FAQ](#-faq)
- [Contributing](#-contributing)
- [License](#-license)

---

## ✨ Why PaperTrail

Most resume builders are online forms that own your data and watermark your PDF. PaperTrail is the opposite:

| | Typical online builder | PaperTrail |
|---|---|---|
| Where your data lives | Their servers | **Your browser only** |
| Cost / account / watermark | Often paid | **Free, none, none** |
| Resume **and** academic CV | Rarely both | **First-class, separate documents** |
| Versioning per company | Manual file chaos | **Built-in snapshots with notes & tags** |
| Tailoring to a JD | Copy-paste guesswork | **Keyword match + one-click injection** |
| Follow-ups & interview reminders | Separate app | **Integrated tracker + bell + toasts** |
| Works on a plane / hostel Wi-Fi | No | **Yes — fully offline** |

---

## 🚀 Quick Start

1. **Download** the single file (`papertrail.html`) from this repository.
2. **Double-click** it — it opens in any modern browser (Chrome / Edge / Firefox).
3. That's it. There is no install, no server, no dependency bundle.

> 💡 Keep the file anywhere you like (Desktop, Drive sync folder, pen drive). Your *data* lives in the browser profile's `localStorage`, not in the file — use **Settings → Workspace backup** to move machines.

<!-- Optional: drop a screenshot here
![Studio overview](docs/screenshots/studio.png)
-->

---

## 🧭 First-Run Flow (recommended)

The in-app **Help & Tour** panel suggests exactly this order:

1. **Reset to a clean page** — start from an empty workspace.
2. **Load the sample data** — a finished industry *Resume* + an academic *CV*, saved versions, tracked applications and a live reminder, so every button has something real to show.
3. **Take the 12-step guided tour**, then experiment freely — edit templates, spacing, exports; the samples are disposable.
4. **Reset again and go real** — fill your own details, save a Master version, export.

---

## 🛠 Feature Guide

### Build & Preview
- Accordion editor: Personal & Contact (+ Scholar/ORCID/interests for CV), Summary, Experience, Education, Publications, Talks, Teaching, Skills, Projects, Certifications, Custom sections.
- Live **A4 preview** in three modes:
  - **Pages** — print-exact pagination with page captions and keep-with-next headings.
  - **Continuous** — one flowing sheet.
  - **Text** — plain-text ATS copy-check.
- Reorder entries by **drag grip** or hover arrows; **move / hide / unhide** whole sections from the preview.
- Slim status line: words · characters · sections · pages · document+template · **Health score**.
- Collapsible toolbar: two tight rows expanded; one scrollable icon row + small stats line collapsed.

### Design & Format
- **4 ATS-safe templates:** Classic Serif · Modern Sans · Compact · Split Column (two-column with divider).
- **Per-type presets:** ATS Ultra-Safe, MNC Classic, Startup Modern, Compact 1-pager, Executive Split · Academic Classic, Research CV, Modern CV, Dense CV.
- 7 font stacks, 6 accent colours, base size, 3 margin presets, and line-height / section-gap / item-gap sliders.
- Every choice is mirrored by the **direct PDF engine** and the print sheet.

### JD Keyword Match
- Paste any job description → frequency + bigram analysis with a large stopword filter.
- Shows **already present** vs **missing** keywords as chips.
- Tap missing keywords and **inject them into a Skills group** in one click.

### Resume Health
- Automatic 9-point audit with a percentage score and fix hints:
  contact completeness · summary length · bullet count · quantified-bullet ratio · skills depth · page limits · file name · saved version · hidden sections.
- Live chip in the status bar; full report in a modal.

### Versions & Snapshots
- **Save** updates the *CURRENT* version (notes-only prompt + replace warning).
- **Save as new** collects target company, comment and tags.
- Identical re-saves are blocked with a confirmation (no duplicate clutter).
- Per-type histories (Resume / CV) with search, sort, tag filters, **CURRENT / LATEST** pills.
- Per version: Load & edit · Preview (Pages/Continuous/Text) · Notes · Edit details · PDF · DOCX · JSON · **ZIP bundle** · Delete.
- Loading a version auto-backs up **only the document being replaced** (toggleable).
- **Document JSON import** creates a new version (optionally loads it into the editor).

### Exports & Bundles
| Export | What it is | Best for |
|---|---|---|
| **PDF (direct)** | Vector PDF written in-browser; selectable text; your template, fonts, margins, spacing | Everyday submissions |
| **PDF (print dialog)** | Browser-rendered A4 sheets → Save as PDF | When exact installed/web font rendering matters |
| **DOCX** | Hand-built OOXML Word file | Portals that demand Word |
| **TXT** | Plain text of the document | ATS copy-paste checks |
| **Document JSON** | One resume *or* CV with styling (`papertrail-document` v1) | Sharing / reusing a single document |
| **Workspace JSON** | Everything: docs, versions, tracker, notifiers, settings | Migration & backup |
| **Bundle ZIP** | PDF + DOCX + Document JSON in one archive | One-click application kit |

- Naming: **Custom** (asks every time, prefilled) or **Timestamp** (`25102026_resume_111432.pdf`).

### Application Tracker + Notifier
- Pipeline: Wishlist → Applied → Screening → Interview → Offer / Rejected, with live stats (total, pipeline, offers, response rate).
- Search, status filters, four sorts, linked document version per application, overdue follow-up flags.
- **Notifier per application:** action label, date, time, advance lead (min/hrs/days), repeat-toasts toggle, toast toggle — reminders stay alive until marked done.

### Bell Notifications
- Top-bar bell with open-count badge and dropdown (due follow-ups + reminder windows).
- Repeating toasts at a configurable interval (15 min – 6 h) with a master on/off switch.
- Each item: **Open application** or **Mark done**.

### Settings, Backups & Safety Copies
- PDF method, naming mode, default preview view, bell toast controls, follow-up default days, auto-backup toggle.
- **Workspace backup / restore** — restore asks *Override everything* vs *Add as new versions*.
- **Local safety copies:** up to 3 rolling snapshots (~every 10 minutes of active work), restorable from Settings.
- Danger zone (confirm-protected): Load sample data · Reset everything.

### Help, Guided Tour & Field Guide
- **Help & Tour:** first-run 4-step card, feature map, daily workflow, and a 12-stop coach-mark tour.
- **Resume Field Guide:** how resumes are read, anatomy, bullet formula + verb bank, company-type tailoring table, ATS rules, length guidance, common mistakes, and an interactive pre-send checklist.

### Mobile Layout
- Bottom navigation: **Build · Versions · Tracker · More** (44 px+ targets).
- **More** bottom-sheet: Settings, Help & tour, Guide, backups, About, Reset (danger-styled, separated).
- Build screen splits into **Edit / Preview / Export** tabs — no cramped side-by-side A4 on phones.

### Fullscreen Studio
- Distraction-free review: design panel + document, exports in an animated **FAB tool menu** (PDF · DOCX · ZIP · Text · JSON · Settings).
- Settings opened from the FAB appears as an **isolated scrollable sheet** (no chrome) with a one-press **Back to fullscreen** return; Esc works too.

---

## 📦 File Formats & Schemas

**Document JSON** (single resume/CV, portable):

```json
{
  "format": "papertrail-document",
  "schemaVersion": 1,
  "documentType": "resume",
  "exportedAt": "2026-10-24T12:00:00.000Z",
  "document": {
    "template": "modern",
    "font": "calibri",
    "accent": "#0c6b58",
    "base": 14,
    "margin": "std",
    "spacing": { "line": 1.42, "sec": 1.2, "item": 0.95 },
    "personal": {},
    "summary": "",
    "experience": [],
    "education": [],
    "skills": [],
    "projects": [],
    "certs": []
  }
}
```

**Workspace JSON** — the full app state (schema-versioned, migrated on import; currently `schemaVersion: 3`).

---

## 🔐 Data & Privacy

- **Zero network calls.** No analytics, no fonts-as-service requirement (system font stacks), no telemetry.
- Everything persists in `localStorage` under one versioned key.
- Three layers of protection: manual **workspace backups**, rolling **local safety copies**, and **auto-backups** before version loads.
- Destructive actions (reset, override-restore, delete) always confirm first.

---

## ⌨️ Keyboard Shortcuts

| Keys | Action |
|---|---|
| `Ctrl / ⌘ + S` | Save version (Save / Save-as dialog) |
| `Ctrl / ⌘ + P` | Download PDF (Build panel) |
| `Esc` | Close modal → end tour → close sheets/menus → exit fullscreen (in that order) |

---

## 🧱 Under the Hood

One HTML file, vanilla ES5-compatible JavaScript, zero libraries:

- **Layout engine** — DOM measurement (`paginate`) drives both the on-screen A4 pages and the print sheet.
- **Vector PDF writer** — builds a real PDF (catalog, pages, Type1 core fonts, xref) with line wrapping computed via `canvas.measureText` in the same font family it embeds; template-aware blocks incl. two-column Split with divider; selectable, ATS-parseable text.
- **ZIP writer** — store-method archive with CRC-32, local headers, central directory and EOCD (used for `.zip` bundles and `.docx`).
- **OOXML generator** — hand-built `word/document.xml` + content types + rels for Word/Google Docs.
- **SVG foreign-object raster path** retired in favour of the vector engine for reliability and selectable text.

Browser support: latest Chrome / Edge / Firefox (desktop & Android); Safari mostly, with print-dialog PDF as fallback.

---

## ✅ ATS Cheat Sheet

- Single column preferred; standard headings; no tables/images carrying information.
- Month YYYY dates (`Mar 2022 – Present`); mirror JD keywords verbatim (JD Match helps).
- 1 page under ~7 years experience, else 2; CVs 2–4 pages.
- Submit **DOCX or selectable-text PDF**; verify with the **Text** view copy-test.

---

## 🗺 Roadmap

- [ ] Export package picker (choose bundle contents)
- [ ] Side-by-side version diff
- [ ] Cover-letter module reusing profile data
- [ ] Web-app manifest + service worker for installable offline use
- [ ] Locale/date-format options

---

## 🙋 FAQ

**Will my resume leave my machine?** No. Everything is local; exports are generated in-browser.

**Can I use it on two computers?** Yes — Settings → Workspace backup → restore on the other machine (or import just one document via Document JSON).

**The portal rejected the direct PDF — now what?** Switch Settings → PDF method to *Print dialog*, or submit the DOCX. Both carry the same content.

**I deleted something by accident.** Entry deletes show an **Undo** toast; older states live in safety copies and versions.

---

## 🤝 Contributing

Issues and pull requests welcome. Keep the golden rules:

1. **Single file**, no build step, no runtime dependencies.
2. **Offline-first** — everything must work from `file://`.
3. **Never break existing data** — bump `SCHEMA` and migrate in `normalize()`.

---

<div align="center">

**Made for job-switchers who refuse to pay a subscription to own their own resume.**
<br/>
⭐ Star the repo if it landed you an interview!
<BR/>
Made with the help of QWEN 3.8 MAX
<BR>
### ⚠️AI CONTENT ⚠️
</div>
