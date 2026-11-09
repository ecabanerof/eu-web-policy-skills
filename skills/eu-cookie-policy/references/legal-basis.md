# Cookies, terminal access, and consent

Baseline checked on 9 November 2026.
Verify the current national rule and guidance for each applicable market at the time of use.

## EU baseline

- Start with [ePrivacy Directive 2002/58/EC, Article 5(3)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:02002L0058-20091219) and [EDPB Guidelines 2/2023 on technical scope](https://www.edpb.europa.eu/our-work-tools/our-documents/guidelines/guidelines-22023-technical-scope-art-53-eprivacy-directive_en).
  Assess actual storage or access on terminal equipment whether or not the information is personal data.
  Confirm any exception for transmission or for operations strictly necessary to provide an information society service explicitly requested by the user.
  Assess each purpose separately and verify local rules before relying on any analytics exception.
- Apply [GDPR Articles 4(11) and 7](https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng/) and the [EDPB consent guidelines](https://www.edpb.europa.eu/documents/guideline/guidelines-052020-on-consent-under-regulation-2016679_en) when consent is required.
  Non-exempt operations require prior valid consent.
  Offer meaningful purpose choices and an accessible withdrawal mechanism, and document consent without collecting unnecessary personal data.
- [CJEU Planet49, C-673/17](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62017CJ0673) rejects preselected consent and addresses disclosures about duration and third-party access.
  Use the [EDPB Cookie Banner Taskforce report](https://www.edpb.europa.eu/documents/task-force-report/report-of-the-work-undertaken-by-the-cookie-banner-taskforce_en) to identify design issues, and check the applicable national position before prescribing an exact first-layer design or wording.
- Draft a layered notice with provider, purpose, category, expiry or duration, third-party access, and how to change or withdraw choices.
  Distinguish tracker lifetime from retention of personal data and the duration of a stored consent choice.
  Link to the privacy notice where the associated processing is explained.

## National starting points

- **Spain.** Check [LSSI Article 22(2)](https://www.boe.es/buscar/act.php?id=BOE-A-2002-13758) and the [AEPD cookie guide](https://www.aepd.es/guias/guia-cookies.pdf).
  Where a consent banner is required, make accepting and rejecting equally easy and comparably visible on the first layer.
  Verify the guide's recommendation on renewing consent within a maximum of 24 months and review sooner if the use changes.
  For a claimed limited audience measurement exemption, check the conditions in the [AEPD audience measurement guide](https://www.aepd.es/guias/guia-cookies-analiticas-externas.pdf) against the actual setup.
- **Germany.** Check [TDDDG §25](https://www.gesetze-im-internet.de/ttdsg/__25.html) and current guidance from the relevant federal or state authority.
  Check the legal basis for subsequent personal-data processing separately.
- **Other markets.** Verify the national transposition and applicable authority guidance.
  Record differences in exemptions, first-layer choices, withdrawal, and renewal before using one implementation across markets.

## Evidence to request

| Consent state | Check on authorized local or staging evidence |
| --- | --- |
| Fresh visit and reject all | No non-exempt terminal operations before consent or after rejection. Check network requests separately for personal-data flows and any terminal access. |
| Accept one purpose | Only operations for that purpose and exempt operations are enabled. Check conditional embeds and tags added through the manager. |
| Accept all | Observed providers, identifiers, purposes and durations agree with the published inventory. |
| Withdraw, then navigate or reload | Previously allowed non-exempt operations stop. Check applicable removal of site-controlled identifiers and what is possible for third-party identifiers. |
| Multiple routes, including embeds | A direct link can be separate from an embedded request. Verify the actual request or storage trigger on each route type. |

Use a clean browser profile and record route, region, build, consent state, observed storage and request timing.
State the limits of static inspection and never infer a live behavior solely from a notice or a tag name.
