# N657CZ Dash Two: Digital Maintenance Manual

This repository contains the structured technical data, inspection procedures, and maintenance manuals (-2) for the **N657CZ** aircraft. 

Unlike a traditional build log, this is a living **Maintenance Manual** designed to provide immediate access to technical specifications and standardized procedures for continued airworthiness.

## ⚙️ Why Markdown for Maintenance?
Traditional formats like Word or Google Docs fail the "Hangar Test." This manual uses Plain Text Markdown because:
* **Portability:** Access technical specs on a tablet, phone, or laptop without needing proprietary software or high-speed internet.
* **Clarity:** Plain text forces a focus on content over formatting, ensuring that critical torque values and clearances are easy to find.
* **Longevity:** These files are future-proof. They will remain readable as long as computers exist, ensuring the aircraft's technical history is never lost to file-format obsolescence.

## 🛠 The Advantage of Git Version Control
Maintenance manuals require strict "Revision Control." Using Git provides:
* **Immutable History:** Every update to a procedure is logged. You can see exactly how a maintenance task evolved over the life of the aircraft.
* **Diff Tracking:** If a specification changes, Git highlights exactly what was modified (e.g., changing a 25-hour inspection to a 50-hour) so nothing is missed.
* **Reliable Backups:** The manual exists on the aircraft's local server ("Hanger") and is mirrored here on GitHub, ensuring redundant access to safety-critical data.

## 🚀 How to Fork This for Your Aircraft
Other builders or owners can use this repository as a framework for their own aircraft-specific maintenance manual.

### 1. Clone the Repository
```bash
git clone [https://github.com/tklenke/OtterWikiN657CZDashTwo.git](https://github.com/tklenke/OtterWikiN657CZDashTwo.git) N-NUMBER-Manual

```

### 2. Standardize Your Manual

* Navigate to the `repository` folder to find the Markdown source files.
* Replace N657CZ-specific data with your own airframe and engine specifications.
* Organise files by system (e.g., `Airframe.md`, `Avionics.md`, `Engine_IO-360.md`).

### 3. Deployment

This repository is designed to be served via **OtterWiki**, providing a searchable, web-based "Wiki" interface in the hangar while maintaining a professional Git backend for revision management.

---

## Disclaimer

The information presented in this documentation is intended for reference purposes only. Users are responsible for verifying the accuracy and applicability of any information provided. The contributors to this wiki are not liable for any consequences resulting from the use or misuse of the information presented. Where information in this wiki is in conflict with FAA AC 43.13-1B, the Plans, the Corrections, or the Newsletters, those documents take precedence.

This manual is specific to N657CZ. Use as a template only; always refer to manufacturer-certified data for your specific components.

---

**License:** MIT
