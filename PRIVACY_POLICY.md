# Privacy Policy for Search Select Extension

**Effective Date:** October 7, 2026  
**Last Updated:** October 7, 2026

## 1. Overview
**Search Select** ("we", "our", or "the extension") is committed to protecting your privacy. This Privacy Policy explains our data practices for the Search Select browser extension.

**In summary: Search Select does NOT collect, track, transmit, or sell any personal data, browsing history, or user identifiers. 100% of your data remains strictly on your local device.**

---

## 2. Information Collection and Use

### A. Personal Data
Search Select does **not** collect any personally identifiable information (PII), such as your name, email address, IP address, device identifier, or location.

### B. Browsing Data & Selection Content
When you use Search Select to select text, links, or images on a webpage:
- Selection processing occurs **entirely inside your local browser instance**.
- No selection queries, URLs, text snippets, or image references are sent to any external server or third-party analytics service by Search Select.
- When you execute a search action, your browser opens standard search engine URLs (e.g., Google, Bing, DuckDuckGo, Brave) directly in a new browser tab, subject to those search providers' respective privacy policies.

### C. Extension Settings & Preferences
Search Select stores user preferences (such as custom search engines, hotkey options, highlight colors, and dark/light mode choices) locally on your device using the standard WebExtensions `chrome.storage.local` API. This data never leaves your device.

---

## 3. Remote Code & Third-Party Dependencies
Search Select does **not** use, execute, or fetch any remote code, external scripts, WebAssembly, or remote CDN resources. All code required for the extension is included within the extension package.

---

## 4. Permissions Justification
The extension requests only the minimum permissions necessary for core functionality:
- `storage`: To save user settings and search engine preferences locally.
- `activeTab` & `scripting`: To display the non-destructive text/image selection highlight overlay on the current active tab when activated by the user.
- `contextMenus`: To add optional right-click options for multi-search.
- `tabs`: To open new search tabs when you execute a search selection.

---

## 5. Third-Party Services
Search Select does not integrate any third-party tracking, advertising, analytics (such as Google Analytics or Mixpanel), or telemetry scripts.

---

## 6. Changes to This Privacy Policy
We may update this Privacy Policy from time to time. Any changes will be reflected in the updated "Effective Date" at the top of this policy.

---

## 7. Contact
If you have any questions or feedback regarding this Privacy Policy, please open an issue on our GitHub repository:  
https://github.com/Deepanshuthakur17/Search-Select-
