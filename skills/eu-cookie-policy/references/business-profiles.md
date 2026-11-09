# Business profiles for cookie policies

Select the profiles that match the site's actual terminal operations.
Use the [cookie template](../assets/cookies-template.md) and verify the applicable market rules in [legal-basis.md](legal-basis.md).
For all profiles, record each identifier or other operation, provider, purpose, lifetime, trigger and applicable choice.
When a server-side tag uses an identifier collected in the browser, classify the browser operation and subsequent disclosure separately.
Use redacted observations and record any unresolved behavior separately.

## SaaS

**Inspect** the public site, sign-in, account settings and authenticated workspace.
Identify session and security mechanisms, user preferences, help widgets, product analytics and any operations added by integrations.

**Draft** sections by purpose and surface.
Verify the exemption for each operation under the local rules, including whether the requested service requires it.
Keep optional product analytics and support tooling separate from necessary sign-in or security operations.
Check whether choices remain effective across public and authenticated domains and after sign-in.

## AI services

**Inspect** the user interface for embedded chat, assistant SDKs, browser storage, device identifiers, pixels and telemetry.
Record what loads on page view, on opening a widget and on sending a request.
Check whether a user action changes the operations and what happens before consent or after refusal where relevant.

**Draft** the actual device-access or storage operations and their purposes.
Assess network disclosures separately from terminal access and route any backend processing of prompts or files to the privacy notice where appropriate.
When relevant to EU ePrivacy, use [EDPB technical scope guidance](https://www.edpb.europa.eu/our-work-tools/our-documents/guidelines/guidelines-22023-technical-scope-art-53-eprivacy-directive_en) to classify the observed mechanism.

## E-commerce

**Inspect** product and cart pages, checkout, payment redirects or embeds, account pages and order confirmation.
Map the domains, operators and control owners for hosted payment and marketplace routes.
Identify cart and payment functions, fraud measures, affiliate attribution, conversion events, advertising and remarketing.

**Draft** actual cart and checkout operations and separate optional tracking by purpose.
Verify any claimed exemption for each operation and market.
Check how third-party domains handle choices and what happens on return from the payment page.
Verify which data the provider receives and keep order details, personal identifiers and payment information out of shared test evidence.

Example inventory row structure for a verified cart mechanism.

| Identifier | Provider | Purpose | Lifetime | Trigger and choice |
| --- | --- | --- | --- | --- |
| {{observed identifier}} | {{verified provider}} | Keeps the products you add in your cart | {{verified lifetime}} | {{observed trigger and applicable choice}} |
