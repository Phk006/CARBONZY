# Deployment Guide

## Current Production URL

```text
https://phk006.github.io/CARBONZY/
```

## Hosting

The app is hosted on GitHub Pages.

Repository:

```text
https://github.com/Phk006/CARBONZY
```

## Publish From Local Repository

Commit changes to `main`:

```bash
git add index.html README.md docs CONTRIBUTING.md SECURITY.md .gitignore .nojekyll
git commit -m "Update CARBONZY documentation"
git push origin main
```

Publish the same version to GitHub Pages:

```bash
git push origin main:gh-pages
```

GitHub Pages serves the app from:

```text
https://phk006.github.io/CARBONZY/
```

## GitHub Pages Settings

If the site does not open:

1. Go to the repository on GitHub.
2. Open **Settings**.
3. Open **Pages**.
4. Set **Source** to **Deploy from a branch**.
5. Select branch **gh-pages**.
6. Select folder **/** root.
7. Save.

GitHub may take a minute or two to publish changes.

## Verification

Check the live URL:

```bash
curl -I https://phk006.github.io/CARBONZY/
```

Expected result:

```text
HTTP/1.1 200 OK
```

## Rollback

Find a previous commit:

```bash
git log --oneline
```

Then publish that commit to `gh-pages`:

```bash
git push origin <commit-sha>:gh-pages --force-with-lease
```

