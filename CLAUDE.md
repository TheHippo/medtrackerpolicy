# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository purpose

This repository contains a single file, `index.md`, the published privacy policy for the MedTracker Android app (developed by Philipp Klose). It is a static document, not a software project — there is no build, lint, or test tooling, and none should be added.

## Related repository

The source code for the MedTracker Android app itself lives at `../MedTracker` (sibling directory), not in this repo. If you need to verify a claim in the privacy policy — e.g. what permissions the app actually requests, what data it stores, or whether it has any network/analytics/crash-reporting code — check `../MedTracker` rather than assuming. That repo also has its own `CLAUDE.md` and a `policy.md` that may be the source of truth this `index.md` is published from; check whether the two need to stay in sync when editing either.

## Site configuration

`_config.yml` configures the GitHub Pages Jekyll build (currently `jekyll-theme-minimal`, plus the page `title`). This is what controls the published page's visual styling — without it, GitHub Pages renders `index.md` as plain unstyled HTML. If you change the theme, pick from GitHub Pages' supported themes list (e.g. `jekyll-theme-cayman`, `jekyll-theme-architect`, `jekyll-theme-minimal`).

## Working with this repository

- The only content is `index.md`. Edits should be factual changes to the privacy policy text (e.g. new permissions, new data practices, contact info changes).
- Whenever the policy content changes in a way that affects what it discloses, update the `**Last updated:**` date at the top of `index.md` to the date of the change.
- Keep claims in the policy accurate to the actual MedTracker app's behavior (data collection, permissions used, local-only storage). Do not add marketing language or claims that can't be verified — this is a legal/compliance document.
- The document is structured as standard sections (Summary, Information We Collect, Information You Enter Into the App, Permissions Used, Data Sharing and Third Parties, Children's Privacy, Data Security, Data Retention and Deletion, Changes to This Policy, Contact). Preserve this structure when editing.
