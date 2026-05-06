# Marketing Automation Platform

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source marketing automation platform for email campaigns, lead nurturing, behavioural triggers, and scoring — without per-contact pricing penalties.

Marketing Automation Platform is a candidate open-source project that brings intent-aware, AI-driven workflow orchestration to teams of any size. It targets B2B demand-generation managers, e-commerce growth marketers, and founders who are priced out of enterprise suites or under-served by today's open-source alternatives. The goal is to combine the data ownership of self-hosted software with the AI capabilities incumbents are only beginning to bolt on.

---

## Why Marketing Automation Platform?

- Commercial suites such as HubSpot Marketing Hub ($20/mo Starter to $3,600/mo Enterprise) and Adobe Marketo Engage ($895–$3,200/mo plus $10k–$50k+ implementation) price on contact count, penalising growth.
- ActiveCampaign and Klaviyo offer strong SMB value but escalate sharply at scale and provide no self-hosting option, leaving customer data on vendor infrastructure.
- The leading open-source incumbent, Mautic (GPL-v3), provides full data ownership but has a dated UI, no AI layer, rules-only lead scoring, and requires significant DevOps effort.
- Existing tools bolt AI onto legacy rule-based engines; intent-aware automation that re-routes contacts mid-journey based on LLM-inferred signals is absent across the market.
- Small teams cannot justify a marketing-ops specialist; automated segment discovery and campaign drafting from natural-language prompts is an unmet need.

---

## Key Features

### Workflow & Campaign Orchestration

- Visual workflow builder with if/then/else logic and branching
- Email campaign creation with template editor (WYSIWYG or HTML)
- Journey canvas with multi-step, multi-channel orchestration
- A/B testing on subject lines and content
- Workflow performance reporting (opens, clicks, conversions)

### Contacts, Segmentation & Scoring

- Contact segmentation with dynamic filter rules
- Lead scoring (rule-based at MVP, predictive/AI-augmented at v1.1)
- Contact import/export with deduplication
- Behavioural tracking across websites, emails, and landing pages
- Account-based marketing (ABM) segmentation

### Multi-Channel Messaging

- Email-first with SMTP compliance and deliverability monitoring
- SMS and WhatsApp channel support
- Behavioural trigger automation (page visits, form fills, time-based)
- Dynamic content personalisation at the individual contact level
- Two-way inbox for inbound messages

### Compliance & Deliverability

- GDPR, CAN-SPAM, and CASL consent tracking
- Bounce handling and deliverability monitoring
- DMARC alignment and BIMI-readiness for verified sender identity
- OAuth 2.0 / OpenID Connect for CRM and third-party integrations

### Integrations & Extensibility

- REST API for campaigns, contacts, emails, and reporting
- Native connectors for HubSpot, Salesforce, and other CRMs
- Webhooks and custom HTTP callouts for event-driven workflows
- Plugin architecture for extending functionality

---

## AI-Native Advantage

Lead scoring today is universally rule-based or built on narrow predictive models; an LLM that synthesises CRM notes, web behaviour, email engagement, and firmographic data can produce explainable scores that outperform current approaches. Intent-aware journey routing, behavioural segment discovery from natural-language prompts, and AI-assisted email copy generation reduce the marketing-ops expertise needed to operate the platform. Compliance automation — inferring consent state from historical engagement — and real-time decisioning at point-of-contact are further AI-native capabilities absent from incumbents.

---

## Tech Stack & Deployment

The project targets a self-hosted open-source deployment model in the spirit of Mautic, with managed cloud as a possible follow-on. Email transmission complies with RFC 5321 (SMTP); integrations use OAuth 2.0 / OpenID Connect; sender identity aligns with DMARC and BIMI. An API-first architecture with webhooks and a plugin system is anticipated, drawing from the Mautic precedent of REST APIs for campaign, contact, email, and report management.

---

## Market Context

The global marketing automation market is estimated at $47B in 2025, projected to reach $81B by 2030 at roughly 11.5% CAGR. Pricing spans from free open-source (Mautic, Listmonk) through $100+/mo SMB SaaS to $100k+/yr enterprise contracts (Marketo, Salesforce Marketing Cloud), with most commercial tools billing by contact count. Primary buyers are B2B demand-generation managers, e-commerce growth marketers, marketing operations specialists, agency account teams, and founders at early-stage SaaS companies.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
