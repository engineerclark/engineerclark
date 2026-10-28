# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

This is the GitHub profile README repository for `engineerclark` (`github.com/engineerclark/engineerclark`). GitHub renders `README.md` from `master` on the user's profile page. There is no build, lint, or test tooling here.

The README is a short preview of Michael's personal website, https://michael.mmclark.org. Its main job is to send visitors to that site. The site's source is at `~/workspaces/mclark/michael_mmclark_org/` (Eleventy), and that source is the source of truth for all content.

## Keeping the README in sync with the site

- Tagline and "Familiar territory" (emoji, name, blurb, `work` id): copy these from `src/_data/site.js` in the site repo. Each item links to `https://michael.mmclark.org/work/#<work id>`. Those ids must exist on the site's `/work/` page.
- Background paragraph: summarize `src/about.md`.
- Use only public content. Never copy private fields from the site's `src/_data/career.js`. That includes employer names, contact details, and private highlights. The site's `lib/privacy.js#toPublic` defines which fields are public.
- Keep only content that rarely changes. Don't list blog posts or projects here, because the README has no way to update itself. Link to `/work/` and `/blog/` instead.

## Conventions

- Badges are local SVG files in `images/badges/`, referenced as `![Name](images/badges/<name>.svg)`. They cover the current core stack, then key earlier skills (C#, TypeScript, JavaScript, Angular, React). To add one, add its SVG to that folder.
- Keep the page short and readable at a glance. Detail belongs on the website.
