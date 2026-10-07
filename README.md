# Search Select

> **Select anything. Search everything.**

Search Select is a productivity-focused browser extension that lets you select text, links, and images on webpages and quickly search or open them.

## ✨ Core Features

- Multi-item selection
- Text, link, and image actions
- Non-destructive selection overlay
- Separate or combined searches
- Google, Bing, DuckDuckGo, Brave, and custom search templates
- Keyboard-first workflow
- Optional context-menu actions
- Configurable settings and themes
- Local browser storage for extension configuration
- No developer-owned browsing-activity backend

### Selection Accuracy

A continuous selection such as `100% offline` is treated as **one selection**, not as individual characters, words, DOM nodes, or spans.

Independent selections such as `React`, `Next.js`, and `GitHub` can be processed as three separate items.

## 🔎 Workflow

**Find something → Select it → Act on it**

Depending on the selected content:

- Text → search
- Link → open/navigate
- Image → image-related search/action
- Multiple items → process independently or use the configured combined-search behavior

## ⌨️ Keyboard Workflow

| Shortcut / Action | Function |
|---|---|
| `Ctrl + S` | Activate selection mode |
| `Ctrl + Shift + S` | Alternate activation |
| `Enter` | Process selected items |
| `Escape` | Exit selection mode |
| `Ctrl + Z` | Undo latest selection/action where supported |

Browser shortcut availability can vary because browser-level shortcuts and other extensions may use the same combinations.

## 🔐 Privacy

Search Select follows a local-first approach.

Selection processing, extension configuration, and optional local history are handled in browser storage/local runtime.

When you explicitly perform a search, the resulting request is sent to the search provider you selected. Search providers have their own privacy policies.

**Privacy Policy:**  
https://github.com/Deepanshuthakur17/Search-Select-PRIVACY_POLICY/blob/main/PRIVACY_POLICY.md

## 🧩 Architecture

```text
Search Select
├── src/
│   ├── background/
│   ├── content/
│   ├── popup/
│   ├── settings/
│   ├── guide/
│   ├── onboarding/
│   ├── lib/
│   └── types/
├── public/
│   ├── manifest.json
│   └── icons/
├── dist/
└── release/
```

## 🔑 Browser Permissions

- **activeTab** — interact with the active webpage after explicit user activation.
- **scripting** — provide webpage selection/interaction functionality.
- **storage** — store extension preferences and configuration locally.
- **contextMenus** — provide optional right-click actions.
- **tabs** — open and manage tabs created by requested search/navigation actions.

## 📦 Development

Requirements:

- Node.js 18+ recommended
- npm 9+ recommended
- Chromium-based browser for primary testing

Install:

```bash
npm install
```

Build:

```bash
npm run build
```

Then open the browser extension management page, enable Developer Mode, choose **Load unpacked**, and select the generated `dist` directory.

## 📦 Edge Release Packaging

The release ZIP must contain `manifest.json` at the ZIP root.

Correct:

```text
Search-Select-v1.0.0.zip
├── manifest.json
├── icons/
├── assets/
└── compiled extension files
```

Do not include another ZIP/CRX inside the package, an unnecessary outer `dist` folder, or unrelated development files.

If configured by the project:

```bash
npm run package:edge
```

## 🌐 Browser Targets

Primary Chromium targets:

- Google Chrome
- Microsoft Edge
- Brave
- Opera

Each target should be runtime-tested independently.

## 🧱 Project Isolation

Search Select must remain isolated from every other browser-extension project.

Do not share:

- `dist`
- manifests
- service workers
- assets
- storage namespaces
- DOM IDs/classes
- CSS namespaces
- message contracts
- build configuration
- release packages

A build or reload of Search Select must never overwrite or modify another extension.

## 🧪 Production Verification

Before publishing, test the actual extension runtime:

- Popup opens
- Selection mode activates
- Text/link/image selection works
- Multiple selections work
- Continuous text is one item
- Search-engine switching works
- Results open correctly
- Context menu works
- Shortcuts work where configured
- Settings persist
- Restricted pages fail safely
- No stale runtime messaging errors
- No unexpected console errors
- No remote executable code
- ZIP root structure is valid

A successful build alone is not considered a complete production test.

## 📬 Support

**Trishul17Tech**  
**Email:** trishul17tech@gmail.com

## 📄 License

Search Select is distributed under a **Production Commercial License** unless a separate license accompanies a release.

Copyright © 2026 Trishul17Tech. All rights reserved.
