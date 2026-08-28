# Maths Training Crash Course 2026 — course website

Source for the course website (GitHub Pages + the *just-the-docs* theme). This
README is for the maintainers (Ali & Sara); it is **not** shown on the website.

## Publishing it (one-time setup, ~5 minutes, no command line needed)

1. Create a new repository on GitHub, e.g. **`cogmaster-maths-2026`**.
   (If you use a different name, open `_config.yml` and change the `baseurl` line to
   `/<your-repo-name>`.)
2. Upload the contents of this folder to the repository:
   on the repo page choose **Add file → Upload files**, drag everything in
   (including the `assets/`, `basic/`, and `advanced/` folders), and commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set
   **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, Save.
4. Wait ~1 minute. Your site is live at
   `https://<your-username>.github.io/cogmaster-maths-2026/`.

## Everyday updates (also possible entirely in the browser)

- **Release a session's solutions:** the solution PDFs are already in
  `assets/basic/solutions/`. Nothing to do — or, if you prefer to hold them back,
  delete the "Solutions" link from a session page until you're ready.
- **Add the Advanced-track materials:** upload Sara's PDFs into `assets/advanced/`
  and edit each `advanced/session-N.md` page (there's a commented-out template with
  the exact link format inside each one).
- **Fill in the schedule:** edit `schedule.md` (dates, times, rooms).
- **Edit any page:** open the `.md` file on GitHub, click the pencil icon, edit, and
  commit. The site rebuilds automatically within a minute.

## Structure

```
_config.yml            site settings + theme + placement-form button
index.md               Home
schedule.md            Schedule & practical info
resources.md           Extra resources / FAQ
basic/                 Basic track (Ali) — overview + 5 session pages
advanced/              Advanced track (Sara) — overview + 5 placeholder pages
assets/basic/          notes, slides, exercises, solutions (PDFs)
assets/advanced/       (Sara's PDFs go here)
```

## Optional: preview locally before publishing

Not required — GitHub builds the site for you. If you *want* a local preview and have
Ruby installed:

```
gem install bundler
bundle install       # uses the included Gemfile
bundle exec jekyll serve
```

## Notes

- GitHub Pages sites are **public**. If you need to restrict access to enrolled
  students, consider hosting on the ENS intranet instead, or keep the URL unlisted.
- Everything is plain Markdown + PDFs — no databases, no maintenance beyond editing
  text files.
