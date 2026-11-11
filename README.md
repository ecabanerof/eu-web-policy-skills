# Website Terms, Privacy Policy, and Cookie Policy Skills

**Web Policy Skills** is an open-source collection of AI agent skills for drafting and reviewing website terms and conditions, privacy policies, and cookie policies in plain English.
Choose the documents you need, describe what your website does, and name the markets you want to cover.
Each skill combines an editable template with prompts for verifying business facts, checking official legal sources, and identifying implementation work.

![A laptop, a world globe, and a stack of tabbed policy documents on a desk](assets/website-policy-drafting-banner.jpg)

Start with the [installation guide](#install-and-use), [choose your markets](#choose-your-scope), or try an [example prompt](#example-prompts).

## Choose an agent skill

Use a European document skill for a focused review of one policy.
Use the global skill for a single market anywhere, a multi-market site, or several policies in one request.

| Skill | Use it for |
| --- | --- |
| [eu-website-terms](skills/eu-website-terms/SKILL.md) | Website terms of use, business disclosures, checkout, consumer sales, subscriptions, cancellation, and withdrawal |
| [eu-privacy-notice](skills/eu-privacy-notice/SKILL.md) | GDPR and other European privacy notices, data processing purposes, retention, recipients, transfers, and rights |
| [eu-cookie-policy](skills/eu-cookie-policy/SKILL.md) | Cookie policies, consent banners, preference controls, and inventories of cookies, pixels, and embeds |
| [global-web-policies](skills/global-web-policies/SKILL.md) | Terms, privacy, or cookies for selected jurisdictions, with shared text and local addenda when needed |

Each skill is an independent folder with a `SKILL.md` entry point, original templates, and supporting references.
The repository is distributed under the [MIT License](LICENSE).

## Choose your scope

Name the markets you want reviewed and which documents you want drafted or audited.
You can select one country, several markets or a worldwide review, and any combination of terms and conditions, privacy policy and cookie policy.
For a market with subnational rules, name the states, provinces or territories you want included.

| Market selection | Where the skill starts |
| --- | --- |
| EU or EEA | EU rules and the applicable national laws of the selected Member States and EEA countries |
| United Kingdom, Switzerland or another European market | The separate local regimes and authorities in the [European jurisdiction guide](JURISDICTIONS.md) |
| United States | Federal and state rules, with [specific starting points for California and New York](skills/global-web-policies/references/united-states.md) |
| Any other country | The [official market sources](skills/global-web-policies/references/market-sources.md) and research into the current law of the named market |
| Multiple markets or worldwide | An applicability map and shared text with local sections for verified differences |

The skill uses your selection to define the work, then checks which rules apply to the actual site, operator and audience.
If you ask for a worldwide review, give the countries you serve or launch first so the skill can prioritise them.
The handover identifies what it verified and which markets or decisions still need evidence.

## Install and use

Download or clone the repository.

```sh
git clone https://github.com/ecabanerof/eu-web-policy-skills.git
```

1. Choose a folder under [`skills/`](skills) and copy the complete folder into your agent's skills directory.
   Keep `SKILL.md`, `assets/`, and `references/` together so the templates and legal sources remain available.
2. In Codex, place the folder in `.agents/skills/` in your project or `~/.agents/skills/` for user-level installation.
   The official documentation lists the supported locations and invocation methods. [Codex skills documentation](https://learn.chatgpt.com/docs/build-skills)
3. Invoke the skill in your agent and describe the website, the markets, and the documents you want.
   For example, ask Codex to use `$global-web-policies` for the privacy and cookie policies of a store serving California and New York.

The skills use Markdown and require no repository runtime dependencies.

## Start with what you know

Describe what your site does, where you operate and who you serve, using everyday language.
You can start before launch or without an existing policy.
The agent asks a short set of questions about material gaps and can prepare a working draft while you confirm the remaining facts.
You can say “I don't know” about a provider, cookie or checkout setting.

> Help me draft the legal pages for my site.
> I run a photography portfolio in Ireland, show work samples and take project enquiries from Ireland and Norway.
> I don't sell through the site and I'm unsure whether the video embeds use tracking.
> Ask me only for the missing facts that matter.

| What your site does | What the skills focus on |
| --- | --- |
| Shows information or a portfolio | Site operator, permitted use, actual data collection and active embeds |
| Takes inquiries, bookings or registrations | The point where data is collected and whether the user is making an inquiry or entering a contract |
| Sells goods, services, downloads or subscriptions | Who sells, what users pay, how the contract ends and which consumer rules apply |
| Sends users to an external seller or hosts a checkout | Who contracts with the user and who controls the payment, confirmation, data and cookie flows |

If you already have policy pages, ask for a review and share the current text or public URLs.
Redacted checkout screenshots, provider lists, retention settings, and cookie inventories help the agent check claims against the live or planned implementation.
Replace credentials, customer records, and other sensitive details with placeholders in any evidence you share.

For all three documents, share the site facts once and expect one group of up to five initial questions.
For Europe-only work, start with `eu-website-terms` for the business model, then reconcile the data and tracker inventory with `eu-privacy-notice` and `eu-cookie-policy`.
For any other single market or a cross-region site, use `global-web-policies` and say where you sell or operate, which legal entities are involved and what choices users currently have.

> Draft our website terms, privacy policy and cookie policy.
> Our site serves customers in the United States, the European Union and Australia.
> We sell through different group companies and use one analytics setup.
> Help us identify what can be shared and what needs its own market section.

## Choose a business profile

Add the profiles that describe the site's actual features.
For example, combine SaaS and AI services for a paid workspace with an AI assistant, and add e-commerce if the site also runs a storefront or checkout.
Artists, musicians, photographers and other professionals can start with the creative and professional sites profile, then add e-commerce for any sales or paid bookings the site actually offers.
Restaurants and food sellers can start with the food profile and add e-commerce for orders, deliveries or paid bookings they offer through their own site or a hosted checkout.
The profiles help the agent ask focused questions and add only the clauses and notices that fit.

| Business profile | What to verify | Guides |
| --- | --- | --- |
| SaaS | Plans, renewals, cancellation, customer workspace data, and product analytics | [Terms](skills/eu-website-terms/references/business-profiles.md#saas) · [Privacy](skills/eu-privacy-notice/references/business-profiles.md#saas) · [Cookies](skills/eu-cookie-policy/references/business-profiles.md#saas) · [Global](skills/global-web-policies/references/business-profiles.md#saas) |
| AI services | Input and output terms, prompts and uploads, model providers, training and retention, and browser widgets | [Terms](skills/eu-website-terms/references/business-profiles.md#ai-services) · [Privacy](skills/eu-privacy-notice/references/business-profiles.md#ai-services) · [Cookies](skills/eu-cookie-policy/references/business-profiles.md#ai-services) · [Global](skills/global-web-policies/references/business-profiles.md#ai-services) |
| E-commerce | Seller, checkout, delivery, withdrawal, payment data, and advertising tags | [Terms](skills/eu-website-terms/references/business-profiles.md#e-commerce) · [Privacy](skills/eu-privacy-notice/references/business-profiles.md#e-commerce) · [Cookies](skills/eu-cookie-policy/references/business-profiles.md#e-commerce) · [Global](skills/global-web-policies/references/business-profiles.md#e-commerce) |
| Creative and professional sites | Portfolios, enquiries, bookings, client galleries, embedded media, and external ticket links | [Terms](skills/eu-website-terms/references/business-profiles.md#creative-and-professional-sites) · [Privacy](skills/eu-privacy-notice/references/business-profiles.md#creative-and-professional-sites) · [Cookies](skills/eu-cookie-policy/references/business-profiles.md#creative-and-professional-sites) · [Global](skills/global-web-policies/references/business-profiles.md#creative-and-professional-sites) |
| Restaurants and food sales | Menus, reservations, allergens, delivery, dietary notes, and ordering tools | [Terms](skills/eu-website-terms/references/business-profiles.md#restaurants-and-food-sales) · [Privacy](skills/eu-privacy-notice/references/business-profiles.md#restaurants-and-food-sales) · [Cookies](skills/eu-cookie-policy/references/business-profiles.md#restaurants-and-food-sales) · [Global](skills/global-web-policies/references/business-profiles.md#restaurants-and-food-sales) |

## Drafting templates

### Website terms and conditions

Build terms around what the site actually offers, from an information-only website to a store with an external checkout or a SaaS subscription.
Check who operates the site, who sells, how an order is accepted, and what the customer sees about price, delivery, renewal, and cancellation.
For consumer sales, use the dedicated withdrawal section where applicable and address voluntary returns and purchase problems in their own sections. [Terms and conditions template](skills/eu-website-terms/assets/terms-template.md) · [Right of withdrawal section](skills/eu-website-terms/assets/terms-template.md#right-of-withdrawal)

### Privacy policy and collection notices

Describe actual processing by purpose, starting with the operator, the data collected, and why it is used.
The privacy skill checks applicable legal bases, recipients, retention, international transfers, and the channels people can use to exercise their rights.
It also helps draft short notices for points of collection such as contact forms, checkout, and account signup. [Privacy policy template](skills/eu-privacy-notice/assets/privacy-template.md)

### Cookie policy, consent banner, and preferences

Inventory what the site loads across analytics, advertising pixels, embedded media, checkout, and other tools.
The cookie skill checks the purpose, provider, trigger, lifetime, and choice for each relevant operation.
Use observed behavior to draft the permanent notice and any required banner, preferences, or opt-out copy. [Cookie policy template](skills/eu-cookie-policy/assets/cookies-template.md)

### Shared policies and market addenda

Use the global template when a single site serves several markets or operates through several legal entities.
Draft shared text where the facts support it and add local sections where the seller, privacy rights, transfer information, or cookie controls differ.
Keep the market decisions and their evidence in the handover table. [Global policy pack template](skills/global-web-policies/assets/policy-pack-template.md)

The templates use conditional sections and fictional or generic examples.
The skills assemble only the sections that fit your site and keep research notes and unresolved facts separate from the proposed public text.
Drafts and reviews are written in plain English.
If a market requires another language for a notice, checkout or consumer document, the review identifies it as a separate publication requirement.

## Example prompts

### Review a privacy policy and cookie policy

> Use global-web-policies to review the privacy and cookie policies for our US storefront.
> We sell in California and New York and use a hosted checkout, an analytics tool, and an advertising pixel.
> Show which policy claims need confirmation from our configuration.

### Draft e-commerce terms for consumer sales

> Use eu-website-terms to draft terms for an online shop selling physical goods to consumers in Ireland.
> Customers pay at checkout and we offer home delivery.
> Include the applicable withdrawal and returns information and identify any checkout details we still need to confirm.

### Draft a privacy notice for SaaS with AI features

> Use eu-privacy-notice for a SaaS workspace that serves business customers in France and Germany.
> Users can upload files to an AI assistant and a separate model provider receives the requests.
> Identify the facts we need to confirm about the provider, retention, training, and international transfers.

### Review a restaurant website

> Use global-web-policies to review the terms, privacy, and cookie pages for a UK restaurant.
> The website displays menus and uses a map and an external table-booking tool.
> Some bookings ask for a deposit and guests can add an optional dietary note.

## What the skills return

1. The requested English draft or a review of the current policy, with proposed changes where appropriate.
2. The markets, facts, and current official sources that support the wording.
3. The implementation checks, such as a withdrawal function, a privacy notice at a form, or a consent control that changes which tags load.
4. The open questions that affect publication, including unverified practices, unresolved local rules, or a required local-language version.

The skills produce editorial and implementation guidance.
Approval of a draft depends on the operator's verified practices, the applicable national rules, and professional review where the decision is material or uncertain.

## Frequently asked questions

### Can I use the skills for a single country?

Yes.
Name the country and any relevant state, province, or territory.
The global skill works for a single market, and the three European skills offer focused entry points for European terms, privacy, and cookies.

### How do the skills handle a worldwide website?

List the markets the business serves or plans to launch in first.
The global skill checks the relevant establishment, audience, and activities and records which markets it could verify.
The [European jurisdiction guide](JURISDICTIONS.md) and [official market sources](skills/global-web-policies/references/market-sources.md) provide starting points for checking national rules.

### Can I use a template without installing a skill?

Yes.
Open the relevant template and fill only the sections that apply to your site.
Use the linked reference material to verify local requirements and tie each claim to the real website or product flow.

### What should I prepare for a cookie policy review?

Provide the relevant page types, a list of tags and providers, and redacted evidence of what loads on first visit and after each available choice.
Include hosted checkout, logged-in pages, or embedded widgets when they use different tools or domains.

### How are contract documents such as a DPA handled?

The SaaS profiles flag when a separate data processing agreement may be needed.
The [privacy policy template](skills/eu-privacy-notice/assets/privacy-template.md) focuses on explaining processing to the people whose data is involved.

## Maintain the references

When changing a legal rule, link to the official consolidated text, decision, or current regulator guidance and record its applicability date.
Check national transposition and, where relevant, EEA incorporation and territorial extent.
Keep examples fictional and keep private project evidence outside this repository.

Open an issue or pull request for a source correction, a new market reference, or an example that reveals a gap in a template.
Include the jurisdiction, the official source, and a short explanation of what changes for the reader.
