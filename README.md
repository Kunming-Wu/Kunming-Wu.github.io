# Kunming-Wu.github.io

Personal homepage of **Wu Kunming (吴坤明)** — M.S. student in Computer Science at Sichuan University.

Live at **https://kunming-wu.github.io**

## What's here

A single hand-written static page. No build step, no framework, no dependencies.

```
index.html              the entire site (markup + CSS + a little JS)
assets/img/avatar.jpg   portrait
assets/img/favicon.svg  site icon
assets/img/logos/       company logos used in the experience section
```

## Features

- **Bilingual** — Chinese and English, toggled with the `EN` / `中文` button in the header.
  Every translatable element carries a `class="zh"` or `class="en"`; CSS shows one and
  hides the other based on `data-lang` on `<html>`.
- **Light / dark theme** — toggled in the header, follows the OS preference on a first visit.
- **Responsive** — single column below 760px; the nav collapses.
- Fully keyboard accessible and respects `prefers-reduced-motion`.

Both preferences persist in `localStorage`.

## Editing

Open `index.html` and change the text. Content is organised top-to-bottom in the order it
renders:

| Section | Anchor |
| --- | --- |
| About | `#about` |
| Education | `#education` |
| Publications | `#publications` |
| Experience | `#experience` |
| Projects | `#projects` |
| Honors & Skills | `#honors` |
| Contact | `#contact` |

Colours and spacing live in the `:root` block at the top of the `<style>` element — edit the
custom properties there rather than the rules below them.

When you add a bilingual paragraph, add both versions side by side:

```html
<span class="zh">中文版本</span>
<span class="en">English version</span>
```

## Deploying

GitHub Pages serves this repository's `main` branch directly — commit and push, and the site
updates in about a minute.

```bash
git add -A
git commit -m "Update homepage"
git push
```
