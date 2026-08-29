# Isaac Davenport

**IT Systems Engineer — macOS fleet management and identity & access at scale.**
Seattle/Tacoma area · 8+ years in enterprise IT

I design and run Apple device fleets and the identity infrastructure behind them.

---

## What I've done

| | |
|---|---|
| **Fleet scale** | Managed macOS fleets from **300 to 2,800+ endpoints** with Jamf Pro and Intune in global enterprise environments |
| **Compliance** | Drove endpoint compliance from **82% → 98%** through automated remediation and smart group engineering |
| **Platform SSO** | Engineered a phased rollout across a Mac fleet, with custom tooling that catches silent enrollment failures. Production against Microsoft Entra ID; validated against Okta in a developer tenant |
| **Automation** | Cut onboarding and provisioning time by **80%** with Jamf workflow automation and Okta lifecycle management (joiner / mover / leaver) |
| **Regulated environments** | **Zero audit findings** across two review cycles on a Federal/DoD GCC High tenant, and full **14-day patching SLAs** under UK Cyber Essentials |
| **AI governance** | Run my organization's AI tool-approval program, governing GitHub Copilot and Claude Code adoption |

---

## Repositories

### Fleet automation

| Repo | What it does |
|---|---|
| [**jamf-toolkit**](https://github.com/IDavenportWA/jamf-toolkit) | Scripts, Extension Attributes and configuration profiles for Jamf Pro. Each tool in its own folder with a README — including the Platform SSO enrollment-gap remediation |
| [**jamf-fleet-toolkit**](https://github.com/IDavenportWA/jamf-fleet-toolkit) | Python automation for Jamf Pro fleet operations: compliance reporting, stale device detection, smart group auditing, policy drift detection. **Read-only by design**, OAuth2 client-credentials auth |
| [**jamf-compliance-bridge**](https://github.com/IDavenportWA/jamf-compliance-bridge) | Syncs Jamf smart-group compliance into Okta and Microsoft Entra ID groups, so Conditional Access and Authentication Policies gate on live device health. **Dry-run by default** |

### Worth a look

Inside `jamf-toolkit`, several tools are built as **pairs** — a control that enforces something, and an Extension Attribute that proves it is working on a given device:

| Control | Verified by |
|---|---|
| [Jamf Connect privilege elevation](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ConfigProfiles/JamfConnectPrivilegeElevation) — 15-minute self-service admin with a mandatory reason | [Elevation reasons](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ExtensionAttributes/PrivilegeElevationReasons) |
| [VS Code extension allowlist](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ConfigProfiles/VSCodeEnterpriseRestrictions) — blocks unapproved AI assistants | [Installed extensions](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ExtensionAttributes/VSCodeExtensions) |
| FileVault enforcement | [Secure token holders](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ExtensionAttributes/SecureTokenUsers) |
| App Auto-Patch | [Per-title patch results](https://github.com/IDavenportWA/jamf-toolkit/tree/main/ExtensionAttributes/AppAutoPatchStatus) |

"The profile is scoped" and "the thing is actually happening on this endpoint" are different claims. Only the second one is evidence.

---

## Toolbox

| Area | |
|---|---|
| **MDM & Endpoint** | Jamf Pro · Platform SSO · Microsoft Intune · Apple Business Manager · macOS security baselines |
| **Identity** | Okta (Certified Professional) · Microsoft Entra ID · Conditional Access · SSO · SCIM provisioning (app-level: Adobe, Expensify, HRIS) · Active Directory |
| **Cloud & Automation** | AWS · Azure · Python · Bash · PowerShell · Docker · Jamf API |
| **ITSM & Collaboration** | Jira · Confluence · ServiceNow · Microsoft 365 · Zoom & Teams Admin |

## Certifications

**Apple/Jamf** — Jamf Certified Tech · Jamf Certified Associate · Jamf Protect Associate
**Identity** — Okta Certified Professional
**Cloud** — AWS Solutions Architect, Developer, SysOps Administrator (Associate) · Azure Administrator (AZ-104)
**Security & Foundations** — CompTIA Security+ · PenTest+ · Cloud+ · Network+ · A+

---

## Elsewhere

🌐 [isaacdavenportwa.dev](https://www.isaacdavenportwa.dev) — case studies, write-ups, and what I'm working on
💼 [LinkedIn](https://www.linkedin.com/in/isaacdavenportwa)
