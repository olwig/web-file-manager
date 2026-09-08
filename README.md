# web-file-manager

Archived web file manager from 15 years ago. My first real, working web project. Left almost as-is; only the old PHP/MySQL/nginx API is now an in-browser simulator (localStorage + SQLite). One repo, offline, new session per browser. Open it, poke around, steal the good bits.

## What this is

The original frontend is HTML, CSS, and JavaScript. Files could be browsed, uploaded, and downloaded against a server API.

The original API ran on nginx with PHP and MySQL. That server stack is **not** in this repo and is **not** hosted here.

## How it runs now

The backend is simulated in the browser so the old UI still works from a single GitHub repo (for example on GitHub Pages):

- API calls stay in the client
- session data lives in `localStorage`
- the database is SQLite in the browser (via sql.js / WASM)

Every visitor has their own isolated data. Nothing is shared. This is an archive and a demo, not a multi-user cloud. It can run offline.

SQL shape and API endpoints were kept as close as possible to the original. Only the transport changed: server PHP became an in-browser simulator.

## Status

Archived. The legacy PHP/MySQL code is not part of this repo. It was translated into the simulator with as little change as possible.

## Goal

Keep the code from rotting in a ZIP. This was my first running web app I was proud of, built without AI.

Public use is fine — see the license (MIT). Fork it, break it, reuse it.

It might come back to life. Back then I already had newer design ideas, mocked up in static Photoshop. I may update it for fun later.
