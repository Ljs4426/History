# Pursuing American Ideals — Unit 8
## AP U.S. History | Luke Sanders | Jacobs HS D300

---

## File Map

| File | Purpose | Embed on Google Sites page |
|---|---|---|
| `widgets/home-hero.html` | Site header, unit intro, 3 lesson nav cards | **Home** |
| `widgets/lesson-55.html` | Reagan exhibit (3 examples + ICED + impact) | **L55: Reagan** |
| `widgets/lesson-56.html` | Cold War exhibit (3 examples + ICED + impact) | **L56: Cold War** |
| `widgets/lesson-59.html` | American Ideals exhibit (3 examples + ICED + impact) | **L59: Ideals** |
| `widgets/quiz.html` | 5-question interactive quiz | **Home** or **Reflection** |
| `full-site/index.html` | Combined single-page preview — open in browser to review | Local preview only |
| `content/site-text.md` | Raw text blocks to paste into Google Sites text sections | All pages |
| `content/sources.md` | Full bibliography with URLs | Reference / Reflection page |

---

## How to Embed in Google Sites

### Step 1: Build the site structure
1. Go to [sites.google.com](https://sites.google.com) → Blank site
2. Title: **Pursuing American Ideals — Unit 8 by Luke Sanders**
3. Add 5 pages in the right-hand panel:
   - Home
   - L55: Reagan
   - L56: Cold War
   - L59: American Ideals
   - Reflection

### Step 2: Embed each widget

On each lesson page:
1. Click **Insert → Embed → Embed code**
2. Open the corresponding widget file (e.g., `widgets/lesson-55.html`) in a text editor
3. Select **all** the text (Ctrl+A / Cmd+A) and copy it
4. Paste into the Google Sites embed dialog
5. Click **Next → Insert**
6. Resize the embed block: drag the bottom edge down until all content is visible (aim for at least 1000px height)
7. Repeat for each lesson page

Embed `widgets/home-hero.html` on the **Home** page.
Embed `widgets/quiz.html` on the **Home** or **Reflection** page.

### Step 3: Update lesson card links

After publishing, the lesson cards in `home-hero.html` need real URLs:

1. Open `widgets/home-hero.html` in a text editor
2. Find the three `href="#lesson-55"`, `href="#lesson-56"`, `href="#lesson-59"` placeholders
3. Replace with your actual published Google Sites page URLs:
   ```
   href="https://sites.google.com/d300.org/yoursite/l55-reagan"
   ```
4. Re-embed the updated `home-hero.html` on the Home page (delete old embed, insert new one)

### Step 4: Add a video

1. Record a 2–3 minute Loom walkthrough of your site at [loom.com](https://loom.com)
2. On the Home page in Google Sites: **Insert → Embed → URL**
3. Paste the Loom share link

### Step 5: Publish

1. Click **Publish** (top right)
2. Set your URL slug (e.g., `pursuing-american-ideals-luke`)
3. Sharing: **Anyone at d300 can view / edit**
4. Copy the published URL and paste it into your teacher's rubric doc

---

## Design Token Reference

| Token | Value | Use |
|---|---|---|
| `--bg` | `#F5F2EB` | Page background (museum wall) |
| `--surface` | `#FFFFFF` | Cards, panels |
| `--ink` | `#1A1A1A` | Body text |
| `--ink-muted` | `#4A4A4A` | Secondary text |
| `--hairline` | `#D9D4C7` | Borders, dividers |
| `--highlight` | `#FFD700` | Impact block top border |
| L55 accent | `#B22234` | Reagan red |
| L56 accent | `#0B3D91` | Federal blue |
| L59 accent | `#6B4423` | Bronze |
| Header font | Playfair Display, serif | All `h1`/`h2`/`h3` |
| Body font | Inter, sans-serif | All paragraph text |
| Mono font | JetBrains Mono | Eyebrows, labels, dates |

---

## Image Attribution

Images were not hardcoded into the widgets to avoid URL rot. To add images:

1. Find free-use images at:
   - Wikimedia Commons: [commons.wikimedia.org](https://commons.wikimedia.org)
   - Library of Congress: [loc.gov/free-to-use](https://www.loc.gov/free-to-use/)
   - National Archives: [archives.gov/research/catalog](https://www.archives.gov/research/catalog)
   - Reagan Library: [reaganlibrary.gov/archives/photographs](https://www.reaganlibrary.gov/archives/photographs)

2. Insert images directly in Google Sites as **Image** blocks above each embed, or add `<img>` tags inside the widget HTML with `onerror` fallbacks:
   ```html
   <img src="[URL]" alt="[description]" 
        onerror="this.style.display='none'"
        style="width:100%;aspect-ratio:16/9;object-fit:cover;border-radius:8px;margin-bottom:24px">
   ```

---

## Known Limitations

| Issue | Workaround |
|---|---|
| Source links inside embeds may be blocked by Google Sites iframe policy | If links don't open, add a text block below each embed listing the sources |
| Google Fonts may not load inside some embeds | System fallbacks (Georgia, system-ui, Courier New) are included and look intentional |
| Embed height: Google Sites iframe clips content | Drag the embed block's bottom edge down; aim for 900–1200px |
| `home-hero.html` lesson card links are placeholders | Update `href` values after publishing (see Step 3 above) |

---

## Pre-Submission Checklist

- [ ] 3 examples per lesson with POV tension and importance/impact
- [ ] ICED-formatted modern connection on each lesson page with cited source
- [ ] At least one video embedded (Loom walkthrough on Home)
- [ ] Interactive element (quiz) embedded
- [ ] Reflection page written in your own voice
- [ ] Site published with "Anyone at d300 can edit" sharing
- [ ] Published URL pasted into teacher's rubric doc
- [ ] Lesson card links updated from `#lesson-XX` placeholders to real URLs
- [ ] Spell-checked

---

*Built with Claude Code | Branch: `claude/build-history-site-widgets-Qaihu`*
