# rahulsrao011.github.io

My personal site. Built with Jekyll and hosted for free on GitHub Pages.

## How to add a blog post

1. Go to the `_posts` folder.
2. Create a new file named `YYYY-MM-DD-some-title.md` (today's date, then a short slug).
   Example: `2026-11-15-what-i-learned-this-week.md`
3. Paste this at the top of the file, then write your post below it in Markdown:

   ```
   ---
   title: What I learned this week
   subtitle: An optional one-line summary.
   tags: [learning]
   ---
   ```

4. Save / commit. The site rebuilds itself in about a minute.

There's a ready-made template in `_drafts/TEMPLATE-copy-me.md` — copy it into `_posts` and rename it.

## How to change your name, tagline, or links

Edit `_config.yml`. Everything editable is at the top of that file.

## How to change the menu (Home / Blog / Projects / About)

Edit the `nav:` list at the bottom of `_config.yml`. To add a new section:

1. Create a file like `notes.md` in the main folder with this at the top:
   ```
   ---
   layout: page
   title: Notes
   permalink: /notes/
   ---
   ```
   and write the page content below it in Markdown.
2. Add it to `nav:` in `_config.yml`:
   ```
     - title: Notes
       url: /notes/
   ```

To remove a section, delete its lines from `nav:` (and optionally delete the file).

## Pages you should edit

| File | What it is |
|---|---|
| `index.md` | Home page — the intro paragraph is marked with a comment |
| `about.md` | About page — placeholder text, rewrite it |
| `projects.md` | Projects page — placeholder projects, replace them |

## Folder guide

| Path | What it is |
|---|---|
| `_config.yml` | Your name, tagline, email, links, and the menu |
| `_posts/` | Your blog posts (one `.md` file each) |
| `_drafts/` | Post template (not published) |
| `assets/` | Images and CSS |
| `_layouts/`, `_includes/` | Page templates (you shouldn't need to touch these) |
