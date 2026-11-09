# Privacy Policy — Personal Tab

**Developer:** Trishul17Tech  
**Effective date:** 9 November 2026  
**Last updated:** 9 November 2026

Personal Tab is a browser new-tab extension that provides a personalized dashboard with a greeting, clock, search box, website shortcuts, and customization controls.

This policy explains how the extension may handle information. The developer must verify every statement against the exact production build before publication.

## 1. Information the Extension Handles

Depending on the features enabled in your installed version, Personal Tab may process:
- Website shortcut names and destination URLs.
- Display preferences, such as appearance, background, layout, and customization settings.
- The current date and time, to display the clock and greeting.
- Search text entered into the search box.

## 2. Local Storage

Personal Tab may use browser extension storage to remember settings and shortcuts between sessions. Confirm the exact storage API and stored fields in the production source code before publishing.

## 3. Search and External Websites

When you submit a search, your search terms are sent to the search provider selected or configured in the extension. That provider may receive your IP address, browser information, and search query under its own privacy policy.

When you open a shortcut, your browser connects to the destination website. That website may collect information according to its own privacy policy.

Personal Tab does not control the privacy practices of external search providers or websites.

## 4. Data Collection and Transmission

Before publication, inspect the production build for analytics, telemetry, remote APIs, crash reporting, advertising, and other network requests. Replace this section with a precise statement based on that inspection.

If the extension does not transmit user data to a developer-controlled server, state that only after verifying it. If it does, identify the data, purpose, recipient, and retention period.

## 5. Browser Permissions

Personal Tab uses browser permissions to provide its implemented features. List each permission from `manifest.json` here and explain its actual purpose before publication. Do not claim permissions are unused without checking the production package.

## 6. Data Sharing

Trishul17Tech does not sell users' personal information. If the production build sends information to an external provider, disclose the provider, information sent, and purpose in this policy and in the browser store's privacy declarations.

## 7. Advertising and Analytics

Inspect the production package for advertising code, analytics SDKs, tracking pixels, and telemetry. This section must accurately state whether any such services are present.

## 8. Data Retention and Deletion

Settings and shortcuts stored by the extension remain in browser extension storage until changed, cleared, or removed. You can generally remove locally stored extension data by clearing the extension's stored data or uninstalling the extension.

External search providers and destination websites may retain information they receive under their own policies.

## 9. Children's Privacy

Personal Tab is a general-purpose productivity and personalization extension. It is not specifically directed at children and should not knowingly collect children's personal information.

## 10. Security

The extension is designed to operate within the browser's extension environment. No software or storage system can guarantee absolute security. Keep your browser updated and install the extension only from a trusted source.

## 11. Changes to This Policy

This policy may be updated when the extension's features, permissions, or data practices change. The updated date will be shown at the top of this document.

## 12. Contact

**Developer:** Trishul17Tech  
**Support email:** trishul17tech@gmail.com

---

**Publisher verification note:** This is a publication draft, not a code audit. Verify storage APIs, permissions, host permissions, network requests, search-provider behavior, background-image sources, analytics, advertising, and third-party services in the exact release ZIP. Make the Microsoft Edge Add-ons privacy disclosures match the verified implementation.
