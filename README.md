# European Web Policy Skills

Three independent, English-language agent skills for drafting and reviewing website terms, privacy policies, and cookie policies across Europe.
Start with the operator's establishment, the markets the site serves, and what the site actually does.
The skills verify EU and national rules across all 27 EU Member States, check incorporation and local rules in Iceland, Liechtenstein and Norway, and use separate legal starting points for the United Kingdom and Switzerland.
For other European markets and territories, they research the applicable local law and regulator before treating a draft as ready for review.
Use the [jurisdiction guide](JURISDICTIONS.md) to find official starting points.

| Skill | Use it for |
| --- | --- |
| [eu-website-terms](skills/eu-website-terms/SKILL.md) | Website terms, trader disclosures, and terms for B2C or B2B transactions |
| [eu-privacy-notice](skills/eu-privacy-notice/SKILL.md) | Privacy notices and a purpose-by-purpose review of processing under the applicable regime |
| [eu-cookie-policy](skills/eu-cookie-policy/SKILL.md) | Cookie and tracker inventories, consent behavior, and notice text |

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
Start with `eu-website-terms` for the business model, then reconcile the data and tracker inventory with `eu-privacy-notice` and `eu-cookie-policy`.
Run each skill independently when you need one document.

## Drafting templates

- [Terms and conditions](skills/eu-website-terms/assets/terms-template.md)
- [Privacy policy and short notices](skills/eu-privacy-notice/assets/privacy-template.md)
- [Cookie policy, banner and preferences](skills/eu-cookie-policy/assets/cookies-template.md)

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
