# Web Policy Skills

English-language agent skills for drafting and reviewing website terms, privacy policies, and cookie policies for European and global sites.
Start with the operator's establishment, the markets the site serves, and what the site actually does.
Use a European document skill for a focused draft or review in Europe.
Use the global skill to coordinate policies across world regions or multinational operations.

| Skill | Use it for |
| --- | --- |
| [eu-website-terms](skills/eu-website-terms/SKILL.md) | Website terms, trader disclosures, and terms for B2C or B2B transactions |
| [eu-privacy-notice](skills/eu-privacy-notice/SKILL.md) | Privacy notices and a purpose-by-purpose review of processing under the applicable regime |
| [eu-cookie-policy](skills/eu-cookie-policy/SKILL.md) | Cookie and tracker inventories, consent behavior, and notice text |
| [global-web-policies](skills/global-web-policies/SKILL.md) | Shared policies and market addenda for companies operating or serving customers across world regions |

## Choose your scope

- **Europe.** The European skills research national rules for all EU Member States, check EEA incorporation and local rules in Iceland, Liechtenstein and Norway, and use separate starting points for the United Kingdom and Switzerland.
  For other European markets and territories, use the [European jurisdiction guide](JURISDICTIONS.md) to find official sources.
- **Global.** The global skill maps where the site operates, sells or processes data, identifies the relevant entities, and separates shared copy from market-specific requirements.
  It uses [official market sources](skills/global-web-policies/references/market-sources.md) and verifies the current law in every market it treats as covered.
  Worldwide availability is one fact to consider alongside actual targeting, sales, establishment and monitoring.

## Install and use

Copy a complete skill folder from `skills/` into your agent's skills directory, including its `assets/` and `references/` folders.
For a user-level Codex installation, use `~/.codex/skills/`.
The repository contains Markdown instructions and original drafting templates.
It needs no runtime dependencies.

## Start with what you know

Describe what your site does, where you operate and who you serve, using everyday language.
You can start before launch or without an existing policy.
The agent asks a short set of questions about material gaps and can prepare a working draft while you confirm the remaining facts.
You can say “I don't know” about a provider, cookie or checkout setting.

> Help me draft the legal pages for my site.
> I run a portfolio in Ireland, show work samples and take project enquiries from Ireland and Norway.
> I don't sell through the site and I'm unsure whether the video embeds use tracking.
> Ask me only for the missing facts that matter.

| What your site does | What the skills focus on |
| --- | --- |
| Shows information or a portfolio | Site operator, permitted use, actual data collection and active embeds |
| Takes inquiries, bookings or registrations | The point where data is collected and whether the user is making an inquiry or entering a contract |
| Sells goods, services, downloads or subscriptions | Who sells, what users pay, how the contract ends and which consumer rules apply |
| Sends users to an external seller or hosts a checkout | Who contracts with the user and who controls the payment, confirmation, data and cookie flows |

Provide redacted policies, inventories or configuration evidence when available.
If you already have pages, ask for a review to see what to keep, change or verify.

For all three documents, share the site facts once and expect one group of up to five initial questions.
For Europe-only work, start with `eu-website-terms` for the business model, then reconcile the data and tracker inventory with `eu-privacy-notice` and `eu-cookie-policy`.
For a cross-region site, use `global-web-policies` and say where you sell or operate, which legal entities are involved and what choices users currently have.

> Draft our website terms, privacy policy and cookie policy.
> Our site serves customers in the United States, the European Union and Australia.
> We sell through different group companies and use one analytics setup.
> Help us identify what can be shared and what needs its own market section.

## Choose a business profile

Add the profiles that describe the site's actual features.
For example, combine SaaS and AI services for a paid workspace with an AI assistant, and add e-commerce if the site also runs a storefront or checkout.
The profiles help the agent ask focused questions and add only the clauses and notices that fit.

| Business profile | Terms and conditions | Privacy policy | Cookie policy | Global sites |
| --- | --- | --- | --- | --- |
| SaaS | [Plans, renewals, cancellation and export](skills/eu-website-terms/references/business-profiles.md#saas) | [Accounts, workspaces and data roles](skills/eu-privacy-notice/references/business-profiles.md#saas) | [Sign-in, sessions and product analytics](skills/eu-cookie-policy/references/business-profiles.md#saas) | [Market-specific SaaS checks](skills/global-web-policies/references/business-profiles.md#saas) |
| AI services | [Inputs, outputs, permitted uses and disclosures](skills/eu-website-terms/references/business-profiles.md#ai-services) | [Prompts, vendors, retention and model improvement](skills/eu-privacy-notice/references/business-profiles.md#ai-services) | [Chat widgets, SDKs and device access](skills/eu-cookie-policy/references/business-profiles.md#ai-services) | [Market-specific AI checks](skills/global-web-policies/references/business-profiles.md#ai-services) |
| E-commerce | [Seller, checkout, delivery and returns](skills/eu-website-terms/references/business-profiles.md#e-commerce) | [Orders, payments, fulfilment and marketing](skills/eu-privacy-notice/references/business-profiles.md#e-commerce) | [Cart, checkout, advertising and embeds](skills/eu-cookie-policy/references/business-profiles.md#e-commerce) | [Market-specific e-commerce checks](skills/global-web-policies/references/business-profiles.md#e-commerce) |

> Draft an English privacy policy for our SaaS with an AI assistant.
> We have account and billing data, users can attach files to chats, and our model provider processes the requests.
> Show which sections can be drafted now and which facts about storage, training and transfers we need to confirm.

## Drafting templates

- [Terms and conditions](skills/eu-website-terms/assets/terms-template.md)
- [Privacy policy and short notices](skills/eu-privacy-notice/assets/privacy-template.md)
- [Cookie policy, banner and preferences](skills/eu-cookie-policy/assets/cookies-template.md)
- [Global policy pack, market addenda and handover matrix](skills/global-web-policies/assets/policy-pack-template.md)

The templates use conditional sections and fictional or generic examples.
The skills assemble only the sections that fit your site and keep research notes and unresolved facts separate from the proposed public text.
Drafts and reviews are written in plain English.
If a market requires another language for a notice, checkout or consumer document, the review identifies it as a separate publication requirement.

## What the skills return

- A document draft or a review of the current text, with material gaps identified.
- The facts, market rules, and source dates that support the result.
- A separate list of technical or business changes and the checks needed to verify them.
- A publication status that distinguishes an evidence-backed draft from one with unresolved prerequisites.

The skills produce editorial and implementation guidance.
Approval of a draft depends on the operator's verified practices, the applicable national rules, and professional review where the decision is material or uncertain.

## Maintain the references

When changing a legal rule, link to the official consolidated text, decision, or current regulator guidance and record its applicability date.
Check national transposition and, where relevant, EEA incorporation and territorial extent.
Keep examples fictional and keep private project evidence outside this repository.

Distributed under the [MIT License](LICENSE).
