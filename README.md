# Knuckles Glass — Site README

## File Structure

```
knucklesglass.com/
│
├── index.html              ← Homepage
├── style.css               ← Shared styles (ALL pages use this)
├── branch-template.html    ← Copy this to create new pages
│
├── glass-lathe.html        ← Branch pages (copied from template)
├── kiln-connect.html
├── glass-art.html
├── puffco-blueprints.html
├── wood-boxes.html
├── dfo-or-bust.html
├── contact.html
│
├── images/                 ← All photos go here
│   ├── lathe-hero.jpg
│   └── ...
│
└── updates/                ← Project update log entries
    ├── glass-lathe/
    │   ├── index.txt       ← List of update filenames (newest first)
    │   ├── 2026-03-01-headstock.md
    │   └── 2026-02-15-motor-mount.md
    ├── kiln-connect/
    │   ├── index.txt
    │   └── ...
    └── ...
```

---

## How to Add a New Update Post

1. Write a new `.md` file in the correct `updates/PAGE-NAME/` folder.

**File format:**
```
---
date: 2026-03-01
title: Headstock is finished
tag: BUILD LOG
---

Write your update here. Plain text works fine.

You can use **bold** and *italic* text.

Add a photo like this:
![Description of photo](../../images/headstock.jpg)

Add a link like this:
[Patreon post](https://patreon.com/yourlink)
```

2. Add the filename to the TOP of `index.txt` in that folder (newest first):
```
2026-03-01-headstock.md
2026-02-15-motor-mount.md
```

3. Drag both files into the correct GitHub folder. Done.

---

## How to Create a New Branch Page

1. Copy `branch-template.html` and rename it (e.g. `glass-lathe.html`)
2. Find and replace `PAGE-NAME` with the actual page name (e.g. `Glass Lathe`)
3. Update `UPDATE_FOLDER` in the script at the bottom to match the updates subfolder
4. Update the hero text, tagline, status badge, intro text, and media
5. Add `class="active"` to this page's nav link
6. Create the matching `updates/page-name/` folder with an empty `index.txt`

---

## How to Update the Instagram Nudge

On `index.html`, find the `ig-nudge` section and update:
- The text inside `.ig-text`
- The `href` on `.ig-link` (can be profile or specific post URL)

---

## Status Badge Classes

| Class | Symbol | Use for |
|-------|--------|---------|
| `status-badge active` | ● | Live / ongoing |
| `status-badge wip`    | ◐ | In progress |
| `status-badge done`   | ○ | Completed |

Add `.earth` for earth-tone color variant.

---

## Changing Colors

Open `style.css` and edit the `:root` block at the top.
Every color on the site references these variables.

---

## Changing Fonts

1. Update the Google Fonts `<link>` URL in each page's `<head>`
2. Update `--font-mono` and `--font-serif` in the `:root` block in `style.css`
