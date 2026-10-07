# signal-music-hosting

A single-file, self-contained React app ("SIGNAL") for hosting and sharing music: artists upload tracks, configure Supabase cloud hosting, and embed a player anywhere.

## Features

- Artist profile: name, bio, avatar URL, settings
- Track uploads as temporary previews or permanent cloud-hosted releases
- Supabase integration: configure project URL, anon key, and bucket name from a settings panel, with a "test connection" button
- Embeddable player: copy-an-embed-code button
- Releases list with title/time metadata
- Toast notifications and a dark, monospace-styled UI

## Tech stack

- Single bundled `index.html` (~200 KB): React 18 via CDN build, Tailwind CSS v3.4.18 (inlined), Lucide icons
- Supabase JS (CDN) for storage/DB when configured
- Deployable statically; `vercel.json` present

## Getting started

No build step — open or deploy `index.html` directly. To enable cloud hosting, enter your Supabase project URL, anon key, and bucket name in the app's Settings panel (nothing is hardcoded).

## Project structure

- `index.html` — the entire app: styles, bundled React code, and app logic in one file
- `vercel.json`, `.vercelignore` — static deploy config

## Status

Working single-file app. The previous README was just "Deploy to Vercel: drag this folder" — functionality above is taken from the UI strings and panels in `index.html`.
