# Multi Links Open

**Select multiple links. Copy them together. Open them with ease.**

Multi Links Open is a browser productivity extension developed by
**Trishul17Tech**. It helps users select multiple hyperlinks on a
webpage and manage them through a simple interface.

## Overview

Managing multiple links individually can be time-consuming. Multi Links
Open makes this process easier by allowing users to select multiple
links and perform actions on them together.

Users can review their selected links, copy their URLs, or open them in
browser tabs.

## Features

### Multi-Link Selection

Select multiple hyperlinks on a webpage using the extension's selection
functionality.

### Copy Selected Links

Copy selected URLs to the clipboard using the Copy action.

### Open Multiple Links

Open selected hyperlinks together using the Open action.

### Selection Counter

View the number of links currently selected.

### Duplicate Handling

Use the duplicate-removal option to avoid repeated URLs, when enabled.

### Flexible Opening Options

Choose from the available opening modes: - Tabs - Pinned tabs - Window

### Link Limit

Configure the maximum number of links to process in one operation, where
supported by the extension settings.

### Keyboard Shortcuts

Use the supported keyboard actions: - **Ctrl + C:** Copy selected
links. - **Enter:** Open selected links.

Shortcut availability may depend on the extension's current state and
browser configuration.

## How to Use

1.  Install Multi Links Open in Microsoft Edge.
2.  Visit a webpage containing hyperlinks.
3.  Activate the extension's link-selection functionality.
4.  Select the links you want to manage.
5.  Review the selected-link count.
6.  Choose **Copy** to copy the selected URLs.
7.  Choose **Open** to open the selected links.
8.  Use the available options to manage how links are opened.

## Installation

### Install from Microsoft Edge Add-ons

Once the extension is published:

1.  Visit its Microsoft Edge Add-ons Store listing.
2.  Select **Get**.
3.  Confirm the installation.
4.  Pin Multi Links Open to your browser toolbar for convenient access.

### Install Manually for Development

1.  Download or clone this repository.

2.  Open a terminal in the project directory.

3.  Install the project dependencies:

    ``` bash
    npm install
    ```

4.  Build the extension using the build script defined in
    `package.json`:

    ``` bash
    npm run build
    ```

5.  Open Microsoft Edge and navigate to:

    ``` text
    edge://extensions
    ```

6.  Enable **Developer mode**.

7.  Select **Load unpacked**.

8.  Choose the generated production folder, normally `dist`, if that is
    the output configured by the project.

**Note:** The actual build command and output directory are determined
by the project's configuration.

## Technology Stack

The exact technologies and dependencies are defined in the project
configuration. This project uses the browser extension platform and its
supported extension APIs.

## Browser Permissions

Multi Links Open may use the following permissions, depending on the
published manifest:

  -----------------------------------------------------------------------
  Permission                          Purpose
  ----------------------------------- -----------------------------------
  `activeTab`                         Temporary access to the active
                                      webpage after user activation

  `scripting`                         Run link-selection functionality on
                                      the webpage

  `tabs`                              Open selected links in browser tabs

  `storage`                           Save supported extension settings

  `contextMenus`                      Provide supported browser
                                      context-menu actions
  -----------------------------------------------------------------------

Refer to `manifest.json` for the permissions included in the actual
release.

## Privacy and Security

Multi Links Open is designed for link selection and management.

For information about webpage access, selected links, storage,
permissions, and data handling, read:

**[Privacy Policy](PRIVACY_POLICY.md)**

## Project Structure

The project structure may vary depending on the current implementation.

Typical files and directories include:

``` text
Multi-Links-Open/
├── public/
├── src/
├── dist/
├── manifest.json
├── package.json
├── README.md
└── PRIVACY_POLICY.md
```

Refer to the actual repository for the complete project structure.

## Development

To work on the project locally:

``` bash
npm install
```

Run the development or build commands defined in `package.json`.

To create a production build:

``` bash
npm run build
```

## Microsoft Edge Add-ons Store

Multi Links Open is intended for distribution through the Microsoft Edge
Add-ons Store.

Store availability depends on Microsoft's review and certification
process.

## License

No open-source license is specified in this repository unless a separate
`LICENSE` file is provided.

All rights and ownership should be determined by the developer's
published licensing terms.

## Developer

**Trishul17Tech**

Product: **Multi Links Open**

------------------------------------------------------------------------

**Multi Links Open --- Manage multiple links with fewer steps.**
