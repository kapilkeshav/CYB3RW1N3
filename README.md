# CYB3RW1N3 — Jekyll Blog for GitHub Pages

This version uses Jekyll, which GitHub Pages builds automatically.

## One-time setup

Open `_config.yml` and replace:

```yaml
github_username: YOUR-USERNAME
```

with your real GitHub username.

If the repository is named `cyb3rw1n3`, set:

```yaml
baseurl: "/cyb3rw1n3"
```

If the repository is named `YOUR-USERNAME.github.io`, leave it as:

```yaml
baseurl: ""
```

## Publish a new blog

1. Copy `post-template.md`.
2. Paste the copy into `_posts`.
3. Rename it:

```text
YYYY-MM-DD-short-title.md
```

Example:

```text
2026-08-05-detecting-powershell.md
```

4. Edit the five metadata values at the top.
5. Paste your article under the second `---`.
6. Save and test.
7. Run:

```bash
git add .
git commit -m "Publish new research post"
git push
```

The landing page automatically creates a card for every file inside `_posts`.

## Important filename rule

Jekyll only recognizes posts using:

```text
YEAR-MONTH-DAY-title.md
```

## Local preview options

### Easiest check

Push to GitHub and check the Pages deployment.

### Full local Jekyll preview

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Open:

```text
http://localhost:4000
```

## GitHub Pages setup

Repository → Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
