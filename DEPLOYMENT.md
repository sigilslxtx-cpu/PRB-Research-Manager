# PRB Research Manager — independent hosting

This is a standalone static web app. It is **not connected to Raw File Rescue**. The hosted application files have no preloaded genealogy records.

## Expected stable address after publishing

GitHub account: `sigilslxtx-cpu`
Repository suggestion: `PRB-Research-Manager`
Expected address (only once published): `https://sigilslxtx-cpu.github.io/PRB-Research-Manager/`

## One-time publishing steps

1. Sign into the intended GitHub account and create a **public** repository named `PRB-Research-Manager`, with its own README or initial commit. GitHub Pages on a free plan requires a public repository. Do NOT create this project inside the existing RFR repository.
2. Upload the **contents** of this folder (not the ZIP file) to the root of that new repository on the `main` branch. Upload `index.html`, `app.js`, `styles.css`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon.svg`, and `.nojekyll`. You may also upload this DEPLOYMENT.md, which contains no private records.
3. In the new repository, open **Settings → Pages**. Set **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**, then Save.
4. When GitHub Pages reports the site is published, open its reported URL and check the Sources, People, Timer, Finances, and Backup screens. The suggested address above is not verified until GitHub confirms it.

## Private data / backup

- NEVER upload `PRB-full-backup-*.json`, `PRB_Genealogy_Drive_Private_Import_*.json`, source attachments, genealogy exports, or other personal data to the public repository.
- PRB uses browser localStorage and IndexedDB for records and attachments. The new HTTPS host uses a **new browser origin**, so it will start with an empty workspace. From the old app, export a complete backup, then restore the backup using **Settings → Restore from JSON backup** at the new site.
- Verify restored counts, individual source records, documents, people, expenses, and archive state BEFORE deleting any old app folder or backup.
- Data stays in the browser for this standalone version; it is not cross-device synchronized and is not suitable for storing sensitive client files on shared computers.
- The site itself is public; access to code is not controlled by a login. Keep backups private and remove them from shared computers.

## Maintenance

- Change service-worker cache version on each release so browsers replace old assets.
- Deploy later versions by replacing the app files in the dedicated repository.
- Maintain separate GitHub history and releases for PRB; never publish it from RFR.
