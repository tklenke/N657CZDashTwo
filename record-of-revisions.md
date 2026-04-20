# Record of Revisions

::: approved
**APPROVED** — 2026-04-17
:::

This manual is maintained as a git repository. Every change to every page is recorded as a commit with a timestamp and description. This provides a complete, auditable history of all revisions.

## Print Footer

Every page of this manual displays a footer when printed showing the date the page was last edited. This date is derived from the git commit that recorded the most recent change to that page.

When working from a printed copy, check the footer date before performing any procedure. To verify the printed copy is current, compare the footer date against the most recent commit for that page:

```
git log -1 --format="%ci %s" -- panels-canopy.md
```

Replace `panels-canopy.md` with the filename of the page (the page name in the URL with `.md` appended). If the commit date is newer than the footer date, the printed copy is out of date — review the current online version before proceeding.

## Recent Changes View

The [[Recent Changes|/-/changelog]] view lists all edits across the entire manual — every page changed, when it was changed, and the description of what changed.

Use this view to:

- Check whether a printed page is current by finding its page name and comparing the date shown against your footer
- Review what has changed since a previous maintenance event
- See the full edit history for any individual page

## Page History

Each page has its own history accessible from the History item in the page menu (top right). The page history lists every revision to that page with timestamps and change descriptions, and allows comparison between any two revisions.

## If You Find an Error

If a procedure or specification in this manual appears to be incorrect, do not rely on it. Flag the issue before performing the work. Corrections are made by editing the page and committing the change, which creates a new revision entry automatically.
