# Privacy Policy — DORA Third-Party Risk Ledger for Jira

**Status:** Draft for Marketplace (P6.3) — publish to a public URL before listing submission.  
**Last updated:** 2026-07-17

## 1. Who we are

This policy covers the Atlassian Forge app **DORA Third-Party Risk Ledger for Jira** (“the App”).

**Controller / publisher:** Najafzadeh Reza (egyéni vállalkozó, Hungary)  
**Contact:** reza@paresh.top

## 2. What the App does

The App helps financial-sector Jira Cloud customers maintain an ICT third-party vendor register and export Register of Information (RoI)–oriented workbooks for DORA-related reporting workflows.

## 3. Data processed

Depending on how you configure and use the App, it may process:

| Category | Examples | Where stored |
|----------|----------|--------------|
| Vendor / ICT third-party records | Name, LEI, criticality, service type, contract dates, governing law, data category, status | Forge Storage (`storage:app`) in your Atlassian cloud |
| Reporting entity details | Legal name, identifiers used in RoI export | Forge Storage |
| Linkage metadata | Issue key ↔ vendor LEI mapping | Forge Storage |
| Audit events | Create/update/delete of vendor records (actor + timestamp) | Forge Storage |
| Jira comments | Link/unlink notices written on issues | Your Jira Cloud site |
| User / group context | Account id, admin flag, membership in `dora-compliance-officers` | Read via Jira APIs; not copied to external systems |

The App does **not** intentionally collect special categories of personal data beyond what you enter into vendor fields (e.g. contact names inside free text). Avoid putting unnecessary personal data into vendor records.

## 4. Purpose and legal basis

Processing is performed to provide the App’s features to your organisation under your Atlassian Cloud agreement and your instructions as the customer. Typical purposes:

- Maintain the ICT third-party ledger
- Link vendors to Jira issues
- Export CSV / RoI Excel for compliance workflows
- Enforce role-based access (admins / compliance officers)

## 5. Where data lives / subprocessors

- App data is stored in **Atlassian Forge Storage** and **Jira Cloud** for your site.
- The App does **not** send vendor or reporting data to the publisher’s own servers.
- Atlassian acts as infrastructure provider under Atlassian’s terms and DPA. See [Atlassian Privacy Policy](https://www.atlassian.com/legal/privacy-policy).

## 6. Access within your organisation

Access is controlled by Jira permissions and App RBAC (e.g. compliance-officer group for export). Your Jira admins manage who can install and use the App.

## 7. Retention and deletion

- Data remains for as long as the App is installed and records are kept by your users.
- Uninstalling the App removes Forge Storage data according to Atlassian Forge retention behaviour for uninstalled apps.
- Jira issue comments remain subject to your Jira retention policies.

## 8. International transfers

Data residency follows your Atlassian Cloud site region and Atlassian’s infrastructure. The App does not introduce additional cross-border transfers outside Atlassian’s platform.

## 9. Your rights

End users should contact their organisation’s Jira / compliance administrators for access, correction, or deletion of App data. Organisations may contact the publisher at the email above for App-related privacy questions.

## 10. Children

The App is intended for business use only and is not directed at children.

## 11. Changes

We may update this policy for Marketplace or legal requirements. The “Last updated” date will change; material changes will be noted in Marketplace release notes where applicable.

## 12. Contact

reza@paresh.top  
Najafzadeh Reza  
Kölcsey út 26., 2721 Pilis, Magyarország
