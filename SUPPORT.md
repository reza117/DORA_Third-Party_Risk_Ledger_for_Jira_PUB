# Support & Docs — DORA Third-Party Risk Ledger for Jira

**Last updated:** 2026-10-15  
**Support email:** reza@paresh.top

Quick guide for Jira admins and compliance users. For legal pages see [Privacy Policy](https://reza117.github.io/DORA_Third-Party_Risk_Ledger_for_Jira_PUB/privacy/) and [Terms of Use](./terms.html).

## 1. What this app does

- Maintain an ICT third-party **vendor ledger** in Jira Cloud (Forge Storage)
- Validate **LEI** format (Mod 97-10)
- Map **subcontracting** chains
- **Link** one Jira issue ↔ one vendor (issue panel is view/link only)
- **CSV** export → Excel → re-import (upsert by LEI)
- **RoI-oriented** Excel export for compliance roles

RoI export is oriented toward EU 2024/2956 / EBA DPM-style fields — **not** claimed as ESA byte-identical official template output. Validate with your compliance team before filing.

## 2. Install

1. Install from Atlassian Marketplace (or your Forge distribution) on a **Jira Cloud** site.
2. Open **Apps → DORA Risk Ledger** (global page).
3. When prompted, **Allow access** so the app can read groups / work items as scoped.

## 3. Create the compliance group (required for RoI)

The app **cannot** create Jira groups. An admin must:

1. Create a **global** group named exactly: `dora-compliance-officers`
2. Add users who may edit **Reporting entity** and run **RoI export**

| Role | Who | Can do |
|------|-----|--------|
| Jira admin | `jira-administrators` | Full config, RoI, reporting entity |
| Compliance | `dora-compliance-officers` | RoI export, reporting entity edit |
| Editor | Users with Edit Issues (typical) | Vendor CRUD, CSV, link/unlink |
| Others | — | Read-only / limited |

## 4. Vendors (global page)

1. Open **DORA Risk Ledger**.
2. **Add vendor** — fill required fields; LEI must pass checksum.
3. Use search / column sort / pagination on the list.
4. **Edit** / **Delete** from the row actions (delete may require edit rights).

**Tip:** Contract expiry shows visual chips (expired / soon). Scheduled email alerts are not included yet.

## 5. Subcontracting

1. Edit a **parent** vendor.
2. Attach direct subcontractors from the vendor picker.
3. Save — the chain appears on the vendor view / RoI export where applicable.

## 6. CSV bulk import / export

1. Global page → **Vendor Bulk import / export**.
2. **Download vendor list (.csv)** or **Download CSV template**.
3. Edit in Excel → save as CSV.
4. Drop/upload the file. Progress shows while import runs in chunks (Forge 25s limit).
5. Re-importing an existing LEI **updates** that vendor.

Large files: expect tens of seconds (e.g. ~50s for ~500 new rows on a typical site).

## 7. Reporting entity & RoI export

1. Fill **Reporting entity** (admin or `dora-compliance-officers`).
2. Click **Export RoI (.xlsx)** — multi-sheet workbook downloads in the browser.
3. Open the file and review sheets before any external use.

Load-tested to ~1000 vendors with RoI export typically under 10 seconds.

## 8. Issue panel (ICT Vendor)

1. Open a Jira issue → **ICT Vendor** panel.
2. Search/select a vendor → **Save** to link (writes a Jira comment).
3. **Unlink** asks for confirmation.
4. Edits to vendor fields are done on the **global page**, not in the panel.

One issue ↔ one vendor (1:1).

## 9. Languages

UI: **English** and **German** (toggle in the app).

## 10. Get help

- Email: **reza@paresh.top**
- Include: site URL, approx. time (UTC), what you clicked, and any error text / request id

## 11. Legal

- [Privacy Policy](https://reza117.github.io/DORA_Third-Party_Risk_Ledger_for_Jira_PUB/privacy/)
- [Terms of Use](./terms.html)
