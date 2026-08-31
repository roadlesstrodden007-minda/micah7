# Micah715

A simple, personal note-taking app for Bible reflections, grocery lists, custom sections, and everything else — built as a single self-contained HTML file, installable to your phone's home screen like a native app.

> *"marvelous things..." — a place for your notes*

### Live Page: https://roadlesstrodden007-minda.github.io/micah7/

## Features

- **Bible Notes** — title, scripture reference, and reflection/study text
- **Grocery** — checklist-style lists with add, check off, and remove items
- **Other** — freeform notes for anything that doesn't fit elsewhere
- **Custom sections** — add your own sections (e.g. "Recipes," "Lyrics," "Journal") as either freeform notes or checklists, each with its own color and icon
- **Move notes between sections** — typed something in the wrong place? Move it to another section and it auto-converts formatting (checklist ↔ text)
- **Search** — search titles, body text, scripture references, and checklist items across every section at once, with color-coded results
- **Scan a screenshot into text (OCR)** — snap or upload a photo/screenshot of typed notes and it's converted to text automatically, with image preprocessing and cleanup for better accuracy
- **Backup & Restore** — download all your notes and custom sections as a single file, and restore them later (handy before clearing your browser or switching devices)
- **Auto-save** — notes save automatically as you type, with a "Saving… / Saved" indicator, and flushes immediately if the app is closed or backgrounded
- **Auto-dated entries** — every note is stamped with the date it was created, shown under the title
- **Installable** — add it to your phone's home screen and it opens full-screen, like a native app
- **No backend, no sign-up** — everything runs client-side in a single HTML file

## Tech Stack

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step
- [Google Fonts](https://fonts.google.com/) (Lora + Inter) loaded via CDN
- [Tesseract.js](https://github.com/naptha/tesseract.js) loaded via CDN, for in-browser OCR (screenshot-to-text)
- Notes, sections, and settings are saved locally in the browser using `localStorage`

## Getting Started

### Run it locally
Just open `index.html` in any modern browser — no installation or server required.

### Install on your phone
Open the live link in your mobile browser:
- **iPhone (Safari):** Share → *Add to Home Screen*
- **Android (Chrome):** ⋮ menu → *Add to Home Screen* / *Install app*

Tap the new icon from your home screen to open it full-screen.

## Using Custom Sections

Tap the **⚙ gear icon** in the header, or the **"+ Section"** chip at the end of the tab row, to:
- Add a new section — give it a name, choose **Notes** (title + body) or **Checklist** (add/check off items), and optionally an emoji icon
- View all your sections with note counts
- Delete a custom section (this also deletes its notes — you'll be warned first)

Built-in sections (Bible Notes, Grocery, Other) can't be deleted, to keep the core app stable.

## Backing Up Your Notes

Since notes are stored per-device (see below), it's worth backing up periodically:
- Tap **⬇ Backup** in the header to download a `.json` file containing all your notes and custom sections
- Tap **⬆ Restore** and select a backup file to load it back in — it won't create duplicates, and adds back any custom sections you don't already have
- To move notes between devices (e.g. phone ↔ laptop), back up on one, transfer the file (email, cloud drive, USB, etc.), then restore on the other

## Data & Storage

Notes are stored locally on your device using the browser's `localStorage`, tied to the specific browser/app instance you're using. Keep in mind:

- Notes **do not sync automatically** across devices or browsers — use Backup/Restore to move them manually
- Clearing your browser's site data, or uninstalling/reinstalling the home screen app, may erase saved notes
- This is intentional for a private, single-device, no-account note app — there is no server storing your data
- The OCR (screenshot scanning) feature also runs entirely in your browser — images are never uploaded anywhere

## Project Structure

```
index.html   — the entire app (markup, styles, and logic in one file)
README.md    — this file
SECURITY.md  — security policy and vulnerability reporting
```

## Roadmap

- Real-time shared grocery lists (planned, requires a small cloud backend — see project notes)

## Credits

Built with [Claude](https://claude.ai).

*Roadlesstrodden*

