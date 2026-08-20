# Micah715

A simple, personal note-taking app for Bible reflections, grocery lists, and everything else — built as a single self-contained HTML file, installable to your phone's home screen like a native app.

> *"walk humbly" — a place for your notes*

## Features

- **Bible Notes** — title, scripture reference, and reflection/study text
- **Grocery** — checklist-style lists with add, check off, and remove items
- **Other** — freeform notes for anything that doesn't fit elsewhere
- **Auto-save** — notes save automatically as you type, with a "Saving… / Saved" indicator
- **Auto-dated entries** — every note is stamped with the date it was created, shown under the title
- **Installable** — add it to your phone's home screen and it opens full-screen, like a native app
- **No backend, no sign-up** — everything runs client-side in a single HTML file

## Tech Stack

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step
- [Google Fonts](https://fonts.google.com/) (Lora + Inter) loaded via CDN
- Notes are saved locally in the browser using `localStorage`

## Getting Started

### Run it locally
Just open `index.html` in any modern browser — no installation or server required.

### Deploy with GitHub Pages
1. Create a new **public** GitHub repository
2. Upload this project's file and name it `index.html` (GitHub Pages serves this by default)
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save
4. After a minute, your live link will appear at the top of that Pages settings screen — something like:
   `https://yourusername.github.io/your-repo-name/`

### Install on your phone
Open the live link in your mobile browser:
- **iPhone (Safari):** Share → *Add to Home Screen*
- **Android (Chrome):** ⋮ menu → *Add to Home Screen* / *Install app*

Tap the new icon from your home screen to open it full-screen.

## Data & Storage

Notes are stored locally on your device using the browser's `localStorage`, tied to the specific browser/app instance you're using. Keep in mind:

- Notes **do not sync** across devices or browsers
- Clearing your browser's site data, or uninstalling/reinstalling the home screen app, may erase saved notes
- This is intentional for a private, single-device, no-account note app — there is no server storing your data

## Project Structure

```
index.html   — the entire app (markup, styles, and logic in one file)
README.md    — this file
```

## Credits

Built with [Claude](https://claude.ai).

*Roadlesstrodden*
