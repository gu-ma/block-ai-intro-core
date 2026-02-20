---
draft: true # Do not publish
---

# How to Use This Class Block Template

This template is designed to help you quickly scaffold and organize class blocks for your course or workshop.

> [!WARNING]
> This template auto-generates `README.md` from `index.md` on push (via GitHub Actions).
> The workflow may create one extra bot commit after your push.
> Before your next push, run `git pull` to avoid non-fast-forward errors.

## README Sync Workflow (GitHub + Quartz)

This template uses a GitHub Actions workflow to keep `README.md` synchronized from `index.md`.

- `index.md` is the source of truth for content.
- On push, the workflow copies `index.md` to `README.md`.
- Frontmatter is removed from `README.md` so GitHub displays it cleanly.
- The workflow commits this update automatically with `github-actions[bot]`.

### What this means for your Git routine

After you push your changes, the workflow may create one additional commit.
Before your next push, run:

```bash
git pull
```

This avoids "branch is behind" / non-fast-forward errors.

## Structure

- **index.md**: Main overview for the block. Update the placeholders `[theme]`, `[block_name]`, `[block_type]` and fill in each section.
- **content/**: Place your main content files here. Use `content_template.md` as a starting point.
- **resources/**: Add any additional resources (links, PDFs, datasets, etc.) here.
- **samples/**: Add sample code, exercises, or solutions here.

## Getting Started

1. Use this template folder for each new block.
2. Update `index.md` with your block's details.
3. Add your content using the provided templates.
4. Place any supporting resources or samples in their respective folders.

## Naming Convention

- Name block repositories using: `block-[theme]-[name]`
- Example: `block-ai-intro-core`

## Tips

- Slides are managed in separated repos (use direct link in your file)
- Keep file and folder names descriptive.
- Remove unused template files as needed.
- Add more sections or templates to fit your teaching style.

---

For questions or suggestions, open an issue or contact the maintainer.
