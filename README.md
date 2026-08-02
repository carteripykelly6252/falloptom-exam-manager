# Falloptom v1.0.0 - browser-based workflow tool 2026

> **Falloptom v1.0.0 is a browser-first, client-side workspace for exam administration and legal research. It is designed for offline operation, stores data in local IndexedDB, and records work in an audit-ready history.**

[![Platform](https://img.shields.io/badge/Platform-web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/carteripykelly6252/falloptom-exam-manager?style=flat-square)](https://github.com/carteripykelly6252/falloptom-exam-manager)

---

<p align="center">
  <a href="https://carteripykelly6252.github.io/falloptom-exam-manager/">
    <img src="https://img.shields.io/badge/Download-Falloptom%20Latest-brightgreen?style=for-the-badge" alt="Download Falloptom">
  </a>
</p>

> **[Download Falloptom v1.0.0](https://carteripykelly6252.github.io/falloptom-exam-manager/)**

---

[Download Latest Build](https://carteripykelly6252.github.io/falloptom-exam-manager/)

---

## What Falloptom Provides

Falloptom is built for browser-based work that requires local ownership of data, consistent organization, and access without an active connection. The application runs in the browser and relies on IndexedDB, avoiding the need for a remote service during routine use.

Its workflow is suited to exam administration and legal research, with tools for organizing work across dedicated tabs, checking for conflicts, and maintaining records that can be reviewed later. The package also contains a US law corpus, advice signing metadata, and an audit chain for documenting the progression of work.

---

## Core Capabilities

- Operates directly in a web browser without a separate desktop installation
- Persists application information in local IndexedDB storage
- Supports workflows that continue while offline
- Offers specialized tabs for exam management
- Includes a bundled corpus of US law for research
- Provides tools for conflict screening
- Adds signing metadata to advice outputs
- Preserves traceability through audit chain records

---

## Getting Started

1. Obtain the source by downloading it or cloning the repository:
   - `git clone https://github.com/carteripykelly6252/falloptom-exam-manager.git
2. Launch the project using the hosted build or by opening the local files in a web browser.
3. For local hosting, serve the files with a basic static web server and visit the application with a current browser.

On the initial launch, Falloptom prepares its local browser data store automatically.

---

## Using the Application

A standard session can follow this sequence:

1. Launch Falloptom in a supported browser.
2. Create new exam records or open existing ones.
3. Consult the included legal corpus through the research tools.
4. Perform conflict screening before completing the work.
5. Inspect signing metadata and audit-chain information when required.
6. Keep using the application offline whenever a network connection is unavailable.

To serve the files locally, run:

- `python -m http.server 8000`

Open the application at:

- `http://localhost:8000`

---

## Local Data and Configuration

Falloptom uses browser storage for its workspace instead of relying on a separate server-side database.

Records and standard application settings are kept in IndexedDB. Where the browser interface provides application-specific options, those preferences are stored with the rest of the local workspace.

The local organization follows this general pattern:

```json
{
  "storage": "IndexedDB",
  "mode": "client-side",
  "offline": true,
  "auditTracking": true
}
```

---

## System Requirements

- A current web browser
- IndexedDB support in that browser
- Sufficient local storage for exam records, legal research content, and audit history
- Optional static hosting or local file serving for access
- No backend runtime is needed for the core browser workflow

---

## Frequently Asked Questions

**How do I install an update?**  
When a newer release is available, use the updated hosted build or replace the local project files with the newer version.

**Where does Falloptom keep my information?**  
The application saves its data in the browser's local IndexedDB storage.

**Does the application work offline?**  
Yes. After the application is available in the browser, it is intended to support work without internet access.

**What should I do if the application fails to load?**  
Use a current browser, reload the application, and clear the site's stored data if necessary. When running locally, also verify that a static server is correctly serving the project files.

**Are workflow options adjustable?**  
Yes. Available configuration is managed through the application interface and saved in local browser storage.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
