# Snippet-Vault

A lightweight, zero-backend productivity tool for storing and instantly accessing frequently used text strings — commands, email templates, links, boilerplate, and anything else you reach for repeatedly.

No accounts. No servers. No setup. Just open the file and go.

---

## What it does

- **Save snippets** with a title and content body
- **Copy in one click** — copies the full content to your clipboard instantly
- **Search in real time** — filters by title or content as you type
- **Edit or delete** any snippet from the card
- **Light / Dark mode** — toggle in the header, preference is remembered
- **Persists across sessions** — all data lives in your browser's `localStorage`

---

## How to use it

**1. Open the file**

Just open `snippet-vault.html` in any modern browser. No installation, no server needed.

```
open snippet-vault.html
```

> If you're on Windows, double-click the file or drag it into a browser window.

**2. Add a snippet**

Click **+ Add Snippet** in the top-right. Give it a title and paste your content. Hit **Save Snippet**.

**3. Copy a snippet**

Click the **Copy** button on any card. The content is copied to your clipboard and a toast confirms it.

**4. Search**

Start typing in the search bar. Cards filter live by title and content.

**5. Edit or Delete**

Use the pencil icon to edit a card, or the trash icon to remove it.

---

## Tech stack

| Layer | Choice |
|---|---|
| Frontend | Vanilla HTML5, CSS3, JavaScript (no frameworks) |
| Storage | Browser `localStorage` |
| Fonts | Outfit (UI) + JetBrains Mono (snippet content) via Google Fonts |
| Deployment | Any static host — GitHub Pages, Vercel, Netlify, or just a local file |

---

## Project structure

```
snippet-vault.html    ← the entire app, single self-contained file
README.md             ← this file
```

Everything — markup, styles, and scripts — lives in one HTML file. There are no dependencies to install and no build step.

---

## Data & privacy

All snippets are stored exclusively in your browser's `localStorage`. Nothing is ever sent to a server. If you clear your browser data or switch browsers, your snippets will not carry over.

To move your snippets to another browser, use your browser's built-in developer tools to export the `snippetvault_v1` key from `localStorage`.

---

## Known limitations

- Data does not sync across devices or browsers
- No export/import yet (planned for a future version)
- `localStorage` storage cap is typically 5 MB per origin

---

## Roadmap

- [ ] JSON export and import for backup and portability
- [ ] Tagging system (Work, Code, Personal, etc.)
- [ ] Keyboard shortcut `Cmd/Ctrl + K` to focus search

---

## Credits

Vibecoded by [@thedatacore](https://twitter.com/thedatacore)
