# TMG Privacy Policy Changelog

This changelog records all material and non-material changes to the Triple Moon Goddess Privacy Policy. Maintained by Claude (Anthropic) on behalf of TMG. Each entry references the policy version, the sections affected, and the nature of the change.

---

## v2026-05d — May 20, 2026

**Reviewed:** May 20, 2026  
**Reviewed by:** Lisa Hagan + Claude (Anthropic)

### Changes

**SFN retired — decision not to use (non-material)**
- `triple-moon-goddess-privacy-sfn.html` created in v2026-05c and immediately retired in this version
- The Mobile Short Form Notice (SFN) requirement comes from a corporate framework document written for large organisations shipping native apps to the Apple App Store and Google Play Store
- TMG is a PWA, not a native app, and has no app store listing
- The full privacy policy (`triple-moon-goddess-privacy-policy.html`) is already written in plain language, is mobile-readable, is linked in every app footer, and covers everything an SFN would summarise
- Maintaining a third privacy document creates ongoing overhead with no user benefit: every policy change would require updating the SFN, the full policy, and the changelog
- The JIT notices handle in-context AI disclosure; the full policy handles everything else
- Decision: one privacy policy, linked in the footer of every app. That is sufficient and correct for TMG’s architecture and scale
- SFN URL now redirects to the full privacy policy to avoid dead links

---

## v2026-05c — May 20, 2026

**Note:** SFN created this version, immediately retired in v2026-05d. See above.

---

## v2026-05b — May 20, 2026

**Reviewed:** May 20, 2026  
**Reviewed by:** Lisa Hagan + Claude (Anthropic)  
**Deployed:** JIT notices confirmed live on dev

### Changes

**Section IV — AI Processing (material)**
- Renamed from “AI Summary Processing” to “AI Processing”
- Added structured table of all three AI touchpoints with location, trigger, data sent, sessionStorage key
- Added callout on sessionStorage expiry behaviour
- Added fifth item to What We Never Do: “Send client names, emails, or birth data to any AI processor”

**Section V — Anthropic processor card (material)**
- Updated to reference summaries and dialog; cross-reference to Section IV table

**Section IX — Cookies and Local Storage (material)**
- Added storage type column; added all three JIT notice sessionStorage keys as explicit rows

**Architecture note: Intents & Permissions document (V) — not applicable (non-material)**
- The project document on Android/iOS intents and permissions was reviewed and determined not applicable to TMG
- TMG apps are PWAs sharing a single Firestore database under one account — the apps are different views on the same data, not separate applications passing data between themselves
- No broadcast intents, no IPC interfaces, no Android permission levels apply
- No policy changes required

---

## v2026-05 — May 20, 2026

**Reviewed:** May 20, 2026  
**Reviewed by:** Lisa Hagan + Claude (Anthropic)

### Changes
- Section I: postal address added (3654 Thornton Ave, Unit #748, Fremont, CA 94536)
- Section IV: AI consent model rewritten (5 free → token opt-in)
- Section IX: cookies table created; `tmg_minor_chart` added
- Section XI: 30-day denial-reason language added
- Section XII: research corpus example and no-PII-in-output statement added
- Section XIV: postal address and 30-day response commitment added
- Hero: effective date corrected to January 1, 2025

---

## v2025-01 — January 1, 2025

**Effective date:** January 1, 2025  
**Note:** Original policy publication. No prior version exists.

### Initial publication covers
- Identity and contact data collection and separation architecture (`user_identities` Firestore collection)
- Health and wellness data as GDPR Article 9 special category
- Legal basis per processing activity (Art 6 and Art 9)
- Third-party processors: Firebase, Anthropic, Google Cloud Run, Google Workspace
- International transfers via SCCs and EU-US Data Privacy Framework
- Data retention table
- Client-side encryption for practitioner apps (XSalsa20-Poly1305 / scrypt)
- Cookies and local storage (strictly necessary only, no advertising trackers)
- Children’s privacy: full platform 18+; age-appropriate natal chart experience for 13–17 with parental consent and local-only storage
- User rights: GDPR (Arts 15–22), CCPA/CPRA, LGPD, PIPEDA, Australian Privacy Act
- Practitioner app data architecture and research corpus pseudonymization
- Contact and complaints: email only (postal address pending at time of publication)

---

## Changelog Maintenance Notes

- This file lives in `TMG-Library` at `legal/PRIVACY_CHANGELOG.md`
- Maintained by Claude (Anthropic) on behalf of Triple Moon Goddess
- **Rule:** The privacy policy HTML and this changelog are always updated in the same session — never one without the other
- **Material changes** = changes that affect how user data is collected, used, shared, or retained
- **Non-material changes** = clarifications, formatting, cross-references, corrections that do not change underlying data practices
- When a new policy version is published, add the entry at the top of this file

## Standing Watch Items

- **Research corpus publication** — review Section XII of the full privacy policy before any research output is published or shared
- **Annual review** — next due May 2027
- **New app added to ecosystem** — triggers policy update at that point
