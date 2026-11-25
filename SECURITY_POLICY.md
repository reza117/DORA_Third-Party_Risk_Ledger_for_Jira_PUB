# Security Policy — DORA Third-Party Risk Ledger for Jira

**Last updated:** 2026-11-25  
**Security contact:** support@paresh.top

This policy describes the security controls, vulnerability management, and incident response for the Atlassian Forge app **DORA Third-Party Risk Ledger for Jira** (“the App”), published by **Najafzadeh Reza** (egyéni vállalkozó, Hungary).

It is separate from the [Privacy Policy](https://reza117.github.io/DORA_Third-Party_Risk_Ledger_for_Jira_PUB/privacy/).

## 1. Security controls

- The App runs as an Atlassian Forge app on the customer’s Jira Cloud site. App code executes on Atlassian’s platform.
- Vendor records, reporting-entity details, issue links, and audit events are stored in Forge Storage and Jira for that site. The publisher does not run a separate server that receives this data.
- Access inside the customer site follows Jira permissions. Register of Information export and reporting-entity edits are limited to Jira administrators and members of the `dora-compliance-officers` group. The customer’s Jira admin creates and maintains that group.
- The App does not ask users for Atlassian passwords. Installation and API access use Atlassian’s Forge authorization.
- Traffic to Jira Cloud uses HTTPS provided by Atlassian.
- Fixes and updates are delivered as new Marketplace versions of the App. Customers should keep the installed version current.

## 2. Vulnerability management

- Report a suspected vulnerability to **support@paresh.top** with the subject line **Security**.
- Include the App version, a description of the issue, and steps to reproduce. Do not send vendor records, exports, or other customer data.
- We acknowledge the report, assess severity, develop a fix, and ship it through the Atlassian Marketplace.
- Please give us a chance to release a fix before any public disclosure.

## 3. Incident response

- If we learn of a vulnerability or incident that could affect customer sites, we investigate, ship a fix or disable the affected behaviour, and email the customer who reported it.
- Where Atlassian Marketplace rules require it, we also notify Atlassian.
- Customer Jira admins remain responsible for who can use the site, who is in `dora-compliance-officers`, and for uninstalling the App. Uninstall removes Forge Storage data according to Atlassian’s retention behaviour.

## 4. Contact

support@paresh.top  
Najafzadeh Reza  
2721 Pilis, Magyarország

Public page: https://reza117.github.io/DORA_Third-Party_Risk_Ledger_for_Jira_PUB/security.html
