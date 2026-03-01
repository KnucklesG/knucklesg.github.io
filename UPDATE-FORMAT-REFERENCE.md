# UPDATE FILE FORMAT REFERENCE
# ════════════════════════════
# Save this file as reference. Do NOT put it in an updates/ folder.
#
# NAMING YOUR FILE:
#   YYYY-MM-DD-short-description.md
#   Example: 2026-03-15-new-burner-installed.md
#
# ADDING IT TO THE SITE:
#   1. Save the .md file to the correct updates/PAGE-NAME/ folder on GitHub
#   2. Add the filename to the TOP of that folder's index.txt
#   3. Done — the page will load it automatically


# ── FULL EXAMPLE FILE ────────────────────────────
---
date: 2026-03-15
title: New oxygen concentrator installed
tag: EQUIPMENT
---

Replaced the old oxygen supply with a dedicated concentrator.
Night and day difference in flame consistency.

You can use **bold** and *italic* text anywhere.

Add a photo like this:
![Description](../../images/your-photo.jpg)

Add a link like this:
[Link text](https://example.com)

Blank lines between paragraphs create new paragraphs automatically.
# ── END EXAMPLE ──────────────────────────────────


# ── FRONTMATTER FIELDS ───────────────────────────
#
#  date   (required) YYYY-MM-DD format
#  title  (required) Short descriptive title
#  tag    (optional) Label shown top-right of entry
#                    Suggested tags:
#                      BUILD LOG
#                      PLANNING
#                      EQUIPMENT
#                      OPEN SOURCE
#                      COLLAB
#                      RELEASE
#                      FIX
#                      NOTE
#
# ── SUPPORTED MARKDOWN ───────────────────────────
#
#  **bold text**
#  *italic text*
#  ![alt text](../../images/filename.jpg)
#  [link text](https://url.com)
#  Blank line = new paragraph
#
# ── IMAGES ───────────────────────────────────────
#
#  Always upload photos to the /images/ folder first.
#  Reference them with the path: ../../images/filename.jpg
#  The ../../ navigates up from updates/PAGE-NAME/ to root.
#
# ── INDEX.TXT FORMAT ─────────────────────────────
#
#  One filename per line, NEWEST FIRST.
#  Lines starting with # are ignored (comments).
#
#  Example index.txt:
#    2026-03-15-concentrator.md
#    2026-03-01-headstock.md
#    2026-01-05-project-start.md
