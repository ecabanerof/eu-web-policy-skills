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

## Creative and professional sites

Use this profile for portfolios, press pages, artist and event sites, client galleries and professional booking pages.
Inventory the relevant surfaces before drafting a single notice.

**Public media.** Distinguish direct links from embedded music or video players, maps and social feeds.
Record what loads on page view and when a visitor chooses to load a feature.
Verify device access, network disclosures and any required choice even when the provider offers a privacy-focused mode.

**Galleries and bookings.** Check private gallery sign-in and access, analytics, external schedulers, ticket widgets and hosted payment routes.
Distinguish the actions needed for a requested service from optional measurement or advertising.
Identify the operator and controls on each relevant domain.

**Draft and verify.** Describe active technologies and applicable controls with verified purposes and lifetimes.
Check first visit, rejection or refusal where offered, activating an embed, and later withdrawal where applicable.
Explain how to change choices using the control that actually exists.
Use the e-commerce profile for payments the operator offers through its own, embedded or hosted checkout.

Example for a verified click-to-load player.

> The {{provider}} player loads when you select {{actual control}}.
> {{Verified description of the operation, its purpose and how to change your choice}}.

## Restaurants and food sales

**Menus and bookings.** Inspect menus, maps, reservation widgets, restaurant platform links and any loyalty or feedback tools.
Record which resources load automatically, which load after user action and which routes take the visitor to another provider.

**Orders and delivery.** For ordering or paid booking, add the e-commerce profile and check carts, checkout and confirmation across domains.
Separate operations needed to complete the requested service from optional measurement, advertising or loyalty features.
Verify the operator, provider, purpose, lifetime and choice mechanism for each operation under the local rules.

**Evidence.** Check first visit and the relevant choice states, including activation of a booking widget and return from a hosted checkout where applicable.
Use redacted local or staging evidence and keep reservation notes, dietary details and payment data out of shared traces.
