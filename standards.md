# Standards & API Reference

> Project: Marketing Automation Platform · Generated: 2026-05-06

## Industry Standards & Specifications

### ISO Standards

- **ISO/IEC 27001:2022 — Information Security Management Systems**
  https://www.iso.org/standard/27001
  Required for SaaS marketing platforms storing PII (subscriber lists, behavioural data); enterprise buyers commonly require ISO 27001 certification before adoption.

- **ISO/IEC 27701:2019 — Privacy Information Management**
  https://www.iso.org/standard/71670.html
  Extension to ISO 27001 for managing PII; aligns with GDPR controller/processor responsibilities for any platform handling subscriber data.

- **ISO/IEC 29100:2024 — Privacy framework**
  https://www.iso.org/standard/85938.html
  Defines a privacy framework relevant to consent capture, opt-in tracking, and data minimisation in marketing workflows.

- **ISO 8601 — Date and Time format**
  https://www.iso.org/iso-8601-date-and-time-format.html
  Used for scheduling sends, journey timing, and event timestamps across APIs and webhooks.

- **ISO 4217 — Currency Codes**
  https://www.iso.org/iso-4217-currency-codes.html
  Required for revenue attribution, e-commerce event payloads, and multi-currency campaign reporting.

- **ISO 639-1 / 639-2 — Language Codes** and **ISO 3166-1 — Country Codes**
  https://www.iso.org/iso-639-language-code  /  https://www.iso.org/iso-3166-country-codes.html
  Used to localise content, segment by geography, and comply with region-specific consent rules.

### W3C & IETF Standards

- **RFC 5321 — Simple Mail Transfer Protocol (SMTP)**
  https://datatracker.ietf.org/doc/html/rfc5321
  Core transport protocol for any email-sending component.

- **RFC 5322 — Internet Message Format**
  https://datatracker.ietf.org/doc/html/rfc5322
  Defines headers (From, Reply-To, List-Unsubscribe) required by mailbox providers.

- **RFC 8058 — One-Click List-Unsubscribe**
  https://datatracker.ietf.org/doc/html/rfc8058
  Mandatory for bulk senders under Gmail/Yahoo 2024 sender requirements.

- **RFC 6376 — DomainKeys Identified Mail (DKIM)**
  https://datatracker.ietf.org/doc/html/rfc6376
  Cryptographic signing of outbound mail; required for deliverability.

- **RFC 7208 — Sender Policy Framework (SPF)**
  https://datatracker.ietf.org/doc/html/rfc7208
  Authorises which servers may send on behalf of a domain.

- **RFC 7489 — Domain-based Message Authentication, Reporting, and Conformance (DMARC)**
  https://datatracker.ietf.org/doc/html/rfc7489
  Required at enforcement (`p=quarantine` or `p=reject`) for BIMI and bulk-sender compliance.

- **BIMI — Brand Indicators for Message Identification (IETF draft / AuthIndicators WG)**
  https://bimigroup.org/  /  https://datatracker.ietf.org/wg/bimi/about/
  Displays verified brand logo in inbox; depends on DMARC enforcement and a Verified Mark Certificate.

- **RFC 6068 — `mailto:` URI scheme**
  https://datatracker.ietf.org/doc/html/rfc6068
  Used in unsubscribe headers and CTA generation.

- **RFC 7231 / RFC 9110 — HTTP Semantics**
  https://datatracker.ietf.org/doc/html/rfc9110
  Underlying spec for REST APIs and webhook delivery semantics.

- **RFC 8288 — Web Linking**
  https://datatracker.ietf.org/doc/html/rfc8288
  Powers pagination patterns used by most marketing platform list APIs.

- **W3C Tracking Preference Expression (DNT) and Global Privacy Control (GPC)**
  https://www.w3.org/TR/tracking-dnt/  /  https://globalprivacycontrol.org/
  Browser signals that consent and behavioural-tracking subsystems should honour.

- **WebSub (W3C Recommendation)**
  https://www.w3.org/TR/websub/
  Pub/sub pattern relevant to webhook fan-out and subscription management.

### Data Model & API Specifications

- **OpenAPI Specification 3.1**
  https://spec.openapis.org/oas/v3.1.0
  De-facto standard for REST API description; most marketing platforms publish OpenAPI documents.

- **AsyncAPI 3.0**
  https://www.asyncapi.com/docs/reference/specification/v3.0.0
  Describes event-driven APIs (webhooks, Kafka, MQTT) — applicable to behavioural trigger streams.

- **JSON Schema (2020-12)**
  https://json-schema.org/
  Validates contact properties, custom event payloads, and template variables.

- **JSON:API 1.1**
  https://jsonapi.org/
  Convention used by some marketing CDPs (e.g. Segment-style) for resource representation.

- **GraphQL (October 2021 spec)**
  https://spec.graphql.org/October2021/
  HubSpot, Shopify and Contentful expose GraphQL endpoints relevant to integrations.

- **CloudEvents 1.0 (CNCF)**
  https://github.com/cloudevents/spec
  Standard envelope for behavioural and transactional event payloads.

- **Webhooks specification (Standard Webhooks)**
  https://www.standardwebhooks.com/
  Emerging convention for signing, retrying, and versioning outbound webhook deliveries.

- **iCalendar (RFC 5545)**
  https://datatracker.ietf.org/doc/html/rfc5545
  Used when journeys include calendar invites (events, demos, meetings).

- **vCard 4.0 (RFC 6350)**
  https://datatracker.ietf.org/doc/html/rfc6350
  Contact import/export format for CRM interoperability.

- **CSV (RFC 4180)**
  https://datatracker.ietf.org/doc/html/rfc4180
  Universal contact list import/export format.

- **MJML / AMP for Email**
  https://mjml.io/  /  https://amp.dev/about/email
  De-facto open standards for responsive email templates and interactive in-mail experiences.

### Security & Authentication Standards

- **OAuth 2.0 (RFC 6749) and OAuth 2.1 (draft)**
  https://datatracker.ietf.org/doc/html/rfc6749  /  https://datatracker.ietf.org/doc/html/draft-ietf-oauth-v2-1
  Standard for third-party CRM, ad-network, and e-commerce integrations.

- **OpenID Connect Core 1.0**
  https://openid.net/specs/openid-connect-core-1_0.html
  SSO for marketer/admin login.

- **SCIM 2.0 (RFC 7643/7644)**
  https://datatracker.ietf.org/doc/html/rfc7644
  Cross-domain identity provisioning — required by enterprise IT for user lifecycle management.

- **OWASP API Security Top 10 (2023)**
  https://owasp.org/API-Security/editions/2023/en/0x11-t10/
  Baseline checklist for marketing-platform API hardening.

- **OWASP ASVS 4.0**
  https://owasp.org/www-project-application-security-verification-standard/
  Application-level controls relevant to subscriber data, form submissions, and webhook security.

- **NIST SP 800-53 Rev. 5**
  https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
  Control families referenced by FedRAMP and large-enterprise security reviews.

- **NIST Cybersecurity Framework 2.0**
  https://www.nist.gov/cyberframework
  High-level governance framework; commonly cited in vendor security questionnaires.

- **GDPR (Regulation (EU) 2016/679)**
  https://gdpr-info.eu/
  Mandates lawful basis, opt-in consent, right of access/erasure, and DPA agreements.

- **CAN-SPAM Act (US, 15 U.S.C. §§ 7701–7713)**
  https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business
  US commercial-email rules: opt-out, sender ID, physical postal address.

- **CASL (Canada)**
  https://crtc.gc.ca/eng/internet/anti.htm
  Express opt-in consent regime stricter than CAN-SPAM.

- **CCPA / CPRA (California)**
  https://oag.ca.gov/privacy/ccpa
  Right-to-know, right-to-delete, opt-out-of-sale obligations affecting subscriber data flows.

- **SOC 2 Type II (AICPA TSC 2017)**
  https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2
  Industry-standard attestation enterprise buyers require.

- **PCI DSS 4.0**
  https://www.pcisecuritystandards.org/document_library/
  Applies if the platform stores or transmits payment card data (e.g. e-commerce attribution).

### MCP Server Specifications

- **Model Context Protocol (MCP)**
  https://modelcontextprotocol.io/  /  https://github.com/modelcontextprotocol
  An MCP server exposing the marketing platform's contacts, segments, journeys, and analytics would let LLM agents draft campaigns, query subscriber state, and trigger sends. Reference servers (filesystem, GitHub, Slack) provide implementation patterns relevant to a marketing-domain server.

- **MCP Tools, Resources, and Prompts primitives**
  https://modelcontextprotocol.io/specification
  Tools for actions (create-campaign, enroll-contact), Resources for read-only data (contact, segment), Prompts for reusable templates (re-engagement journey, win-back sequence).

## Similar Products — Developer Documentation & APIs

### HubSpot
- **Description:** All-in-one marketing, sales, and CRM platform with deep automation and content tools.
- **API Documentation:** https://developers.hubspot.com/docs/api/overview
- **SDKs/Libraries:** Node.js, Python, Ruby, PHP, .NET — https://github.com/HubSpot
- **Developer Guide:** https://developers.hubspot.com/docs/api/intro-to-auth
- **Standards:** REST/JSON, GraphQL (CRM), OpenAPI 3.x, Standard Webhooks-style signed deliveries
- **Authentication:** OAuth 2.0, Private App tokens

### Adobe Marketo Engage
- **Description:** Enterprise B2B marketing automation with ABM, scoring, and revenue attribution.
- **API Documentation:** https://developer.adobe.com/marketo-apis/
- **SDKs/Libraries:** Community Python (`marketorestpython`), Node clients; no official multi-language SDK
- **Developer Guide:** https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/marketo-rest-api
- **Standards:** REST/JSON, SOAP (legacy), Munchkin tracking JS
- **Authentication:** OAuth 2.0 (custom service apps)

### ActiveCampaign
- **Description:** SMB-focused automation with visual workflow builder and built-in CRM.
- **API Documentation:** https://developers.activecampaign.com/reference/overview
- **SDKs/Libraries:** Community PHP, Node, Python clients
- **Developer Guide:** https://developers.activecampaign.com/docs
- **Standards:** REST/JSON, OpenAPI-style reference
- **Authentication:** API Key (URL + key pair)

### Klaviyo
- **Description:** E-commerce-focused email/SMS automation with predictive analytics.
- **API Documentation:** https://developers.klaviyo.com/en/reference/api_overview
- **SDKs/Libraries:** Official Python, PHP, Node, Ruby, Java, .NET — https://github.com/klaviyo
- **Developer Guide:** https://developers.klaviyo.com/en/docs/welcome
- **Standards:** REST/JSON, JSON:API resource format, OpenAPI spec published
- **Authentication:** OAuth 2.0 (newer), Private API Key

### Brevo (Sendinblue)
- **Description:** Multi-channel automation: email, SMS, WhatsApp, chat, CRM with EU data residency.
- **API Documentation:** https://developers.brevo.com/reference/getting-started-1
- **SDKs/Libraries:** Official Node, PHP, Python, Ruby, Java, C#, Go — https://github.com/getbrevo
- **Developer Guide:** https://developers.brevo.com/docs
- **Standards:** REST/JSON, OpenAPI 3.0
- **Authentication:** API Key (`api-key` header)

### Mautic (Open Source)
- **Description:** Self-hostable marketing automation with email, lead scoring, journeys.
- **API Documentation:** https://developer.mautic.org/
- **SDKs/Libraries:** Official PHP, community Node/Python — https://github.com/mautic/api-library
- **Developer Guide:** https://developer.mautic.org/#rest-api
- **Standards:** REST/JSON, JSON:API-ish responses
- **Authentication:** OAuth 2.0, Basic Auth

### Customer.io
- **Description:** Developer-friendly event-driven messaging across email, push, SMS, webhooks.
- **API Documentation:** https://docs.customer.io/api/
- **SDKs/Libraries:** Official Node, Python, Ruby, Go, Java, mobile SDKs (iOS/Android) — https://github.com/customerio
- **Developer Guide:** https://customer.io/docs/api/
- **Standards:** REST/JSON; Track API + App API split; webhooks with HMAC signing
- **Authentication:** Basic Auth (Site ID + API Key), Bearer tokens

### Iterable
- **Description:** Cross-channel automation for email, SMS, push, in-app, web push.
- **API Documentation:** https://api.iterable.com/api/docs
- **SDKs/Libraries:** Official Node, Python, Ruby, mobile SDKs
- **Developer Guide:** https://support.iterable.com/hc/en-us/categories/204158108-Developer-Hub
- **Standards:** REST/JSON, OpenAPI document
- **Authentication:** API Key (server / mobile / JWT-authenticated keys)

### Braze
- **Description:** Cross-channel customer engagement (email, push, in-app, SMS, content cards).
- **API Documentation:** https://www.braze.com/docs/api/basics/
- **SDKs/Libraries:** Web, iOS, Android, React Native, Flutter, Unity SDKs — https://github.com/braze-inc
- **Developer Guide:** https://www.braze.com/docs/developer_guide/
- **Standards:** REST/JSON, OpenAPI; Currents data export uses CloudEvents-style schemas
- **Authentication:** REST API Key (Bearer)

### Salesforce Marketing Cloud (Account Engagement / Pardot)
- **Description:** Enterprise marketing automation tightly integrated with Salesforce CRM.
- **API Documentation:** https://developer.salesforce.com/docs/marketing/pardot/guide/intro.html
- **SDKs/Libraries:** Salesforce CLI, FuelSDK (legacy), language wrappers community-maintained
- **Developer Guide:** https://developer.salesforce.com/docs/marketing
- **Standards:** REST/JSON, SOAP (legacy SFMC), Salesforce Object Query Language (SOQL)
- **Authentication:** OAuth 2.0 with Salesforce Connected Apps

### Listmonk (Open Source)
- **Description:** Lightweight self-hosted newsletter and mailing-list manager.
- **API Documentation:** https://listmonk.app/docs/apis/apis/
- **SDKs/Libraries:** None official; REST API consumable directly
- **Developer Guide:** https://listmonk.app/docs/
- **Standards:** REST/JSON
- **Authentication:** Basic Auth, API users with tokens

### Segment (CDP, adjacent)
- **Description:** Customer data platform that feeds marketing-automation tools with unified events.
- **API Documentation:** https://segment.com/docs/api/
- **SDKs/Libraries:** Analytics.js, mobile SDKs, server-side libraries in 10+ languages — https://github.com/segmentio
- **Developer Guide:** https://segment.com/docs/connections/sources/catalog/libraries/
- **Standards:** REST/JSON, Spec for `track`/`identify`/`page` events (de-facto industry pattern), OpenAPI for Public API
- **Authentication:** Write Key (sources), OAuth 2.0 / Personal Access Token (Public API)

## Notes

- **Sender requirements (Gmail/Yahoo, Feb 2024):** Bulk senders (>5,000/day) must implement SPF + DKIM + DMARC, one-click unsubscribe (RFC 8058), and keep spam complaint rate below 0.3%. Any new platform must enforce these by default at onboarding.
- **MCP for marketing is nascent:** No widely adopted reference MCP server for marketing automation exists yet; this is a green-field opportunity to define a canonical server schema (contacts, segments, journeys, campaigns, events).
- **Webhook standardisation is fragmented:** Most platforms invented their own signing/retry semantics; the Standard Webhooks initiative (https://www.standardwebhooks.com/) is the most credible convergence effort and is worth adopting.
- **AMP for Email adoption is uneven:** Gmail and Yahoo support it; Apple Mail and Outlook do not. Treat as progressive enhancement.
- **Privacy regimes are diverging:** GDPR (EU), CCPA/CPRA (California), CASL (Canada), LGPD (Brazil), POPIA (South Africa), India's DPDP Act 2023 — multi-jurisdiction consent state machines are increasingly required.
- **Cookieless future:** Third-party cookie deprecation in Chrome (ongoing) is shifting tracking toward server-side events (Conversions API, Enhanced Conversions, CAPI) — server-event ingestion endpoints should be first-class, not afterthoughts.
