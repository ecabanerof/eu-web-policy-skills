# EU Web Policy Skills

Three independent agent skills to draft or review website terms, privacy notices, and cookie notices for an EU context.
The skills use official legal sources, verified facts about the site, and the rules of the relevant Member States.
Spain and Germany have starter references.
For other Member States, the skills require research against the relevant national law and regulator before treating a country-specific issue as resolved.
Operators established outside the EU can use the skills to assess when EU rules apply to their activities.
The coverage is limited to EU rules and their relevant national implementation.

| Skill | Use it for |
| --- | --- |
| [eu-website-terms](skills/eu-website-terms/SKILL.md) | Website terms, trader disclosures, and terms for B2C or B2B transactions |
| [eu-privacy-notice](skills/eu-privacy-notice/SKILL.md) | GDPR privacy notices and a purpose-by-purpose review of processing |
| [eu-cookie-policy](skills/eu-cookie-policy/SKILL.md) | Cookie and tracker inventories, consent behavior, and notice text |

## Install and use

Copy a complete skill folder from `skills/` into your agent's skills directory, including its `references/` folder.
For a user-level Codex installation, use `~/.codex/skills/`.
The repository contains Markdown instructions and needs no runtime dependencies.

Start by giving the agent the operator's establishment, target markets, audience, actual features, and existing policies.
Provide redacted inventories or configuration evidence when available.
Ask for an audit first when you are unsure what the site does in practice.

> Use eu-cookie-policy to review our Spanish portfolio site.
> We have a contact link, a video embed, and a consent manager.
> Review our current notice and consent configuration, then separate proposed copy changes from implementation checks.
> Reply in Spanish.

When reviewing all three documents, classify the business with `eu-website-terms` first, then reconcile the data flows and tracker inventory with `eu-privacy-notice` and `eu-cookie-policy`.
Run each skill independently when you need one document.

## What the skills return

- A document draft or a review of the current text, with material gaps identified.
- The facts, market rules, and source dates that support the result.
- A separate list of technical or business changes and the checks needed to verify them.
- A publication status that distinguishes an evidence-backed draft from one with unresolved prerequisites.

The skills produce editorial and implementation guidance.
Approval of a draft depends on the operator's verified practices, the applicable national rules, and professional review where the decision is material or uncertain.

## En español

Indica desde dónde opera el titular, a qué países se dirige, qué funciones están activas y qué documentos quieres revisar.
Puedes pedir una revisión, un borrador, o ambos.
Los datos del sitio y las dudas de publicación quedan separados de las referencias legales y del texto propuesto.

## Maintain the references

When changing a legal rule, link to the official consolidated text, decision, or current regulator guidance and record its applicability date.
Check the national transposition when a rule comes from a directive.
Keep examples fictional and keep private project evidence outside this repository.

Distributed under the [MIT License](LICENSE).
