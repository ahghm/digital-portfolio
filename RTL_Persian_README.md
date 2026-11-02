# Persian RTL version

This version adds `_static/custom.css` and configures the Jupyter Book to use it.

## Build locally

From the project root:

```bash
jupyter-book build .
```

The generated website is normally in:

```text
_build/html/
```

Open:

```text
_build/html/intro.html
```

## Publish to GitHub Pages

After checking the local build, commit and push the project:

```bash
git add .
git commit -m "Add Persian RTL styling and responsive typography"
git push origin main
```

If your GitHub Pages workflow/build is already configured, the site should redeploy automatically.

## Notes

- Persian text is RTL and right-aligned.
- Vazirmatn is used as the primary Persian font.
- Code and notebook outputs remain LTR.
- Images remain responsive.
- The CSS is centralized in `_static/custom.css`, so future Markdown/notebook edits do not require adding RTL formatting to every paragraph.
