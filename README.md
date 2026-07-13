# contextual-build-artifacts

Update manifests for Contextual desktop apps, served via GitHub Pages at
**https://build-artifacts.contextual.io**.

- `/apps.json` — index of apps, their latest versions, and human download links
- `/<app>/latest.json` — per-app [Tauri updater](https://v2.tauri.app/plugin/updater/) manifest (the URL baked into each app)

Contents are published by each app's release CI (e.g. `ContextualIO/ctxl-tool`).
Update payloads are minisign-verified by the apps themselves — this host serves
pointers, not trust.
