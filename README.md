# Awesome Agentic Commerce: Protocols, Payments and Tools (2026) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of the protocols, SDKs, payment providers, open source implementations, research and current developments behind agentic commerce: AI agents that discover, compare and buy on behalf of people and businesses ([what is agentic commerce?](https://www.agentic-commerce.sh/en/guides/what-is-agentic-commerce/)). Updated daily. Vendor-neutral: it covers protocols, payments, agents, research and standards, not shop systems.

Every protocol entry links to its specification, repository, licence and released version, and was checked against the published sources on **2026-11-09**. The list is generated from the data behind [agentic-commerce.sh](https://www.agentic-commerce.sh/), where each protocol has a full profile with an example flow and sources. Last updated: **2026-11-27**.

## Contents

- [Start here](#start-here)
- [Protocols](#protocols)
- [SDKs](#sdks)
- [Reference implementations and test suites](#reference-implementations-and-test-suites)
- [Payments for agents](#payments-for-agents)
- [Agent identity and verification](#agent-identity-and-verification)
- [Shopping agents and assistants](#shopping-agents-and-assistants)
- [Open source experiments](#open-source-experiments)
- [Research, benchmarks and data](#research-benchmarks-and-data)
- [Tools for merchants](#tools-for-merchants)
- [Standards bodies and communities](#standards-bodies-and-communities)
- [Recent developments](#recent-developments)
- [Books and long reads](#books-and-long-reads)
- [Related lists](#related-lists)
- [Contributing](#contributing)

## Start here

- [What is agentic commerce?](https://www.agentic-commerce.sh/en/guides/what-is-agentic-commerce/) - Definition, a purchase in three steps and current examples.
- [UCP, MCP and ACP compared: Choosing protocols for your shop](https://www.agentic-commerce.sh/en/guides/ucp-mcp-acp-comparison/) - Which protocol does which job in a shop.
- [How do agentic checkout and payments work?](https://www.agentic-commerce.sh/en/guides/agentic-checkout-and-payments/) - How an agent checks out and pays.
- [Agentic commerce examples for merchants](https://www.agentic-commerce.sh/en/guides/agentic-commerce-examples/) - Examples by industry.
- [Which payment providers support purchases by AI agents?](https://www.agentic-commerce.sh/en/guides/payment-providers-for-agent-purchases/) - Card networks and payment providers for agent purchases compared.
- [How can a shop tell approved shopping agents from bots?](https://www.agentic-commerce.sh/en/guides/tell-shopping-agents-from-bots/) - Web Bot Auth and how a shop recognises approved agents.
- [Agentic commerce statistics 2026: What do the numbers show?](https://www.agentic-commerce.sh/en/guides/agentic-commerce-statistics/) - Key figures with source and date.
- [Glossary](https://www.agentic-commerce.sh/en/glossary/) - Agentic commerce terms from A to Z.

## Protocols

### Commerce & checkout

| Protocol | Status | Specification | Source | Licence | Profile |
| --- | --- | --- | --- | --- | --- |
| **ACP** · Agentic Commerce Protocol | Beta · Snapshot 2026-04-17 | [Spec](https://www.agenticcommerce.dev/docs) | [Repo](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) | Apache-2.0 for the official repository; check community libraries separately. | [Profile](https://www.agentic-commerce.sh/en/protocols/acp/) |
| **UCP** · Universal Commerce Protocol | Released · v2026-08-25 | [Spec](https://ucp.dev/specification/overview/) | [Repo](https://github.com/Universal-Commerce-Protocol/ucp) | Apache-2.0 | [Profile](https://www.agentic-commerce.sh/en/protocols/ucp/) |

### Mandates, identity & customer access

| Protocol | Status | Specification | Source | Licence | Profile |
| --- | --- | --- | --- | --- | --- |
| **AP2** · Agent Payments Protocol | Released · 0.2.0 | [Spec](https://ap2-protocol.org/) | [Repo](https://github.com/google-agentic-commerce/AP2) | Apache-2.0 | [Profile](https://www.agentic-commerce.sh/en/protocols/ap2/) |
| **Visa TAP** · Trusted Agent Protocol | Documented · Official sample | [Spec](https://developer.visa.com/docs/trusted-agent-protocol/trusted-agent-protocol-specifications) | [Repo](https://github.com/visa/trusted-agent-protocol) | Visa Developer Center Terms and TAP Product Terms; not licensed under MIT or Apache. | [Profile](https://www.agentic-commerce.sh/en/protocols/tap/) |
| **Verifiable Intent** · Verifiable Intent | Draft v0.1 · Reference SDK alpha | [Spec](https://verifiableintent.dev/) | [Repo](https://github.com/agent-intent/verifiable-intent) | Apache-2.0 | [Profile](https://www.agentic-commerce.sh/en/protocols/verifiable-intent/) |
| **Poppy** · Personal Agent Protocol | Published draft 0.1 · Draft 0.2 in progress | [Spec](https://personalagentprotocol.org/docs/spec) | [Repo](https://github.com/personal-agent-protocol/personal-agent-protocol) | Apache-2.0 for the specification and documentation; trademarks, logos and design are excluded. Datalayer community SDKs: BSD-3-Clause. | [Profile](https://www.agentic-commerce.sh/en/protocols/poppy/) |
| **PACT** · Personal Agent Consent & Trust | Early project · A2A extension | [Spec](https://openpactprotocol.org/) | [Repo](https://github.com/openpactprotocol/openpactprotocol) | Apache-2.0 | [Profile](https://www.agentic-commerce.sh/en/protocols/pact/) |

### Machine payments

| Protocol | Status | Specification | Source | Licence | Profile |
| --- | --- | --- | --- | --- | --- |
| **x402** · x402 Payment Protocol | Specification family v2 | [Spec](https://x402.org/) | [Repo](https://github.com/x402-foundation/x402) | Apache-2.0 | [Profile](https://www.agentic-commerce.sh/en/protocols/x402/) |
| **MPP** · Machine Payments Protocol | Active project · IETF draft expired | [Spec](https://mpp.dev/) | [Repo](https://github.com/tempoxyz/mpp-specs) | Repository specifications: CC0 1.0; repository tooling: MIT OR Apache-2.0. IETF documents follow IETF Trust rules; SDKs use their respective package licences. | [Profile](https://www.agentic-commerce.sh/en/protocols/mpp/) |
| **L402** · Lightning based API payments and authentication | Specification with published JavaScript SDKs | [Spec](https://github.com/lightninglabs/L402) | [Repo](https://github.com/lightninglabs/L402) | L402sdk: MIT OR Apache-2.0. Terms for the specification and other implementations are in their respective repositories. | [Profile](https://www.agentic-commerce.sh/en/protocols/l402/) |
| **ATXP** · Agent Transaction Protocol | SDKs and integrations | [Spec](https://github.com/atxp-dev) | [Repo](https://github.com/atxp-dev/sdk) | MIT for SDK and integration packages; separate service terms apply to the hosted service. | [Profile](https://www.agentic-commerce.sh/en/protocols/atxp/) |

### Transport & tools

| Protocol | Status | Specification | Source | Licence | Profile |
| --- | --- | --- | --- | --- | --- |
| **MCP** · Model Context Protocol | Revision 2026-07-28 | [Spec](https://modelcontextprotocol.io/docs/2026-07-28/learn/versioning) | [Repo](https://github.com/modelcontextprotocol/modelcontextprotocol) | Transition from MIT to Apache-2.0: new code and specification contributions use Apache-2.0; older contributions not yet relicensed remain MIT. Documentation outside the specification: CC-BY-4.0. SDKs have their own licence files. | [Profile](https://www.agentic-commerce.sh/en/protocols/mcp/) |
| **A2A** · Agent2Agent Protocol | Released · v1.0.1 | [Spec](https://a2a-protocol.org/) | [Repo](https://github.com/a2aproject/A2A) | Apache-2.0 for the protocol repository; check SDK licences separately. | [Profile](https://www.agentic-commerce.sh/en/protocols/a2a/) |
| **WebMCP** · structured browser tools | Experimental · Community Group Draft | [Spec](https://webmachinelearning.github.io/webmcp/) | [Repo](https://github.com/webmachinelearning/webmcp) | Specification: W3C Community Contributor License Agreement (CLA); check implementations separately. | [Profile](https://www.agentic-commerce.sh/en/protocols/webmcp/) |

### Experience & interface

| Protocol | Status | Specification | Source | Licence | Profile |
| --- | --- | --- | --- | --- | --- |
| **AXP** · Agentic Experience Protocol | Early project · README version 2026-01-13 | [Spec](https://github.com/agentic-commerce-lab/AXP-protocol) | [Repo](https://github.com/agentic-commerce-lab/AXP-protocol) | The README states Apache-2.0; check the precise licence scope before redistribution. | [Profile](https://www.agentic-commerce.sh/en/protocols/axp/) |
| **MCP Apps** · MCP Apps Extension | Stable specification · 2026-01-26 | [Spec](https://modelcontextprotocol.io/extensions/apps/overview) | [Repo](https://github.com/modelcontextprotocol/ext-apps) | Repository transitioning from MIT to Apache-2.0; some older contributions remain MIT. Documentation outside the specification: CC-BY-4.0. Package metadata still lists MIT; consult the licence files of the release used. | [Profile](https://www.agentic-commerce.sh/en/protocols/mcp-apps/) |

## SDKs

Official and maintained community SDKs, as listed in each protocol profile.

**ACP**

- [Official specification](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol/tree/main/spec/2026-04-17) -  · official
- [Svix ACP Models](https://github.com/svix/agentic-commerce-protocol) - TypeScript, Python, Rust, Ruby, Go, Java, Kotlin · `agentic-commerce-protocol`
- [Shopbridge PHP](https://github.com/shopbridge/shopbridge-php) - PHP · `shopbridge/shopbridge-php`

**UCP**

- [UCP JavaScript SDK](https://github.com/Universal-Commerce-Protocol/js-sdk) - TypeScript, JavaScript · `@ucp-js/sdk` · official
- [UCP Python SDK](https://github.com/Universal-Commerce-Protocol/python-sdk) - Python · `ucp-sdk` · official
- [UCP PHP SDK · Core](https://github.com/agentic-commerce-alliance/ucp-php-sdk-core) - PHP · `ucp-php-sdk/core`
- [UCP PHP SDK · Symfony bundle](https://github.com/agentic-commerce-alliance/ucp-php-sdk-symfony-bundle) - PHP · `ucp-php-sdk/symfony-bundle`

**AP2**

- [AP2 Python reference SDK](https://github.com/google-agentic-commerce/AP2/blob/main/code/sdk/python/ap2/sdk/README.md) - Python · `code/sdk/python/ap2` · official

**Visa TAP**

- [Visa TAP sample system](https://github.com/visa/trusted-agent-protocol) - Python, JavaScript · official

**Verifiable Intent**

- [Verifiable Intent Python](https://github.com/agent-intent/verifiable-intent) - Python · `verifiable-intent` · official

**x402**

- [x402 reference implementations](https://github.com/x402-foundation/x402) - TypeScript, Python, Go · `@x402/core; x402; github.com/x402-foundation/x402/go/v2` · official
- [x402 Java](https://github.com/x402-foundation/x402/tree/main/java) - Java · `org.x402:x402:1.0.0-SNAPSHOT` · official

**MPP**

- [mppx](https://github.com/wevm/mppx) - TypeScript · `mppx` · official
- [pympp](https://github.com/tempoxyz/pympp) - Python · `pympp` · official
- [mpp-go](https://github.com/tempoxyz/mpp-go) - Go · `github.com/tempoxyz/mpp-go` · official
- [mpp-rs](https://github.com/tempoxyz/mpp-rs) - Rust · `mpp` · official
- [mpp-rb](https://github.com/stripe/mpp-rb) - Ruby · `mpp-rb` · official

**Poppy**

- [Official Company Kit](https://github.com/personal-agent-protocol/personal-agent-protocol) -  · `kit/company im Repository` · official
- [Datalayer Personal Agent Protocol](https://github.com/datalayer/personal-agent-protocol) - Python, TypeScript · `personal-agent-protocol; @datalayer/personal-agent-protocol`

**PACT**

- [PACT TypeScript packages](https://github.com/openpactprotocol/openpactprotocol) - TypeScript · `@openpactprotocol/protocol; @openpactprotocol/client` · official

**MCP**

- [MCP TypeScript v2](https://github.com/modelcontextprotocol/typescript-sdk) - TypeScript, JavaScript · `@modelcontextprotocol/server; @modelcontextprotocol/client` · official
- [MCP Python](https://github.com/modelcontextprotocol/python-sdk) - Python · `mcp` · official
- [MCP PHP](https://github.com/modelcontextprotocol/php-sdk) - PHP · `mcp/sdk` · official
- [MCP Rust](https://github.com/modelcontextprotocol/rust-sdk) - Rust · `rmcp` · official
- [MCP Go](https://github.com/modelcontextprotocol/go-sdk) - Go · `github.com/modelcontextprotocol/go-sdk/mcp` · official
- [MCP .NET](https://github.com/modelcontextprotocol/csharp-sdk) - .NET · `ModelContextProtocol` · official
- [MCP Java](https://github.com/modelcontextprotocol/java-sdk) - Java · `io.modelcontextprotocol.sdk:mcp` · official

**A2A**

- [A2A JavaScript](https://github.com/a2aproject/a2a-js) - TypeScript, JavaScript · `@a2a-js/sdk` · official
- [A2A Python](https://github.com/a2aproject/a2a-python) - Python · `a2a-sdk` · official
- [A2A Rust](https://github.com/a2aproject/a2a-rs) - Rust · `a2a-lf; a2a-client-lf; a2a-server-lf` · official
- [A2A Go](https://github.com/a2aproject/a2a-go) - Go · `github.com/a2aproject/a2a-go/v2` · official
- [A2A .NET](https://github.com/a2aproject/a2a-dotnet) - .NET · `A2A` · official
- [A2A Java](https://github.com/a2aproject/a2a-java) - Java · `org.a2aproject.sdk:a2a-java-sdk-reference-jsonrpc` · official

**AXP**

- [AXP schemas and services](https://github.com/agentic-commerce-lab/AXP-protocol) -  · official

**MCP Apps**

- [MCP Apps SDK](https://github.com/modelcontextprotocol/ext-apps) - TypeScript · `@modelcontextprotocol/ext-apps` · official

**L402**

- [L402 JavaScript SDKs](https://github.com/lightninglabs/L402sdk) - TypeScript, JavaScript · `@lightninglabs/l402; @lightninglabs/l402-ai` · official
- [L402 Rust core and language bindings](https://github.com/lightninglabs/L402sdk) - Rust, Go, Python · official

**ATXP**

- [ATXP SDK](https://github.com/atxp-dev/sdk) - TypeScript, JavaScript · `@atxp/client; @atxp/server; @atxp/express; @atxp/x402` · official

## Reference implementations and test suites

Samples, validators and conformance tests published by the protocol projects themselves.

- [UCP samples](https://github.com/Universal-Commerce-Protocol/samples) - Official sample implementations for the Universal Commerce Protocol.
- [UCP conformance tests](https://github.com/Universal-Commerce-Protocol/conformance) - Test suite to check a UCP implementation against the specification.
- [UCP schema validator](https://github.com/Universal-Commerce-Protocol/ucp-schema) - Validates UCP documents against the published schemas.
- [AP2](https://github.com/google-agentic-commerce/AP2) - Agent Payments Protocol specification, reference code and samples for mandates.
- [A2A x402 extension](https://github.com/google-agentic-commerce/a2a-x402) - Adds x402 crypto payments to agent-to-agent conversations.
- [x402](https://github.com/x402-foundation/x402) - HTTP-native payments: specification and reference packages from the x402 Foundation.
- [Visa Trusted Agent Protocol sample](https://github.com/visa/trusted-agent-protocol) - Sample merchant and agent flow for signed, identifiable shopping agents.
- [MCP reference servers](https://github.com/modelcontextprotocol/servers) - Reference servers that show how tools and data are exposed through MCP.
- [A2A samples](https://github.com/a2aproject/a2a-samples) - Sample agents and clients for the Agent2Agent protocol.
- [A2A CLI](https://github.com/a2aproject/a2a-cli) - Official command line client for testing A2A-compatible agents.

## Payments for agents

Developer resources from networks and payment providers for purchases that an agent initiates. A comparison is in the [payment providers guide](https://www.agentic-commerce.sh/en/guides/payment-providers-for-agent-purchases/).

- [Visa Intelligent Commerce](https://developer.visa.com/capabilities/visa-intelligent-commerce) - Visa's developer programme for agent-initiated card payments. [Analysis](https://www.agentic-commerce.sh/en/news/visa-agentic-ready-akzeptanz/)
- [Mastercard Agent Pay with Ant International](https://www.ant-intl.com/en/news/detail/mastercard-and-ant-international-advance-trusted-agentic-commerce-in-asia-pacific/) - Agent payments tested with Antom in Asia Pacific. [Analysis](https://www.agentic-commerce.sh/en/news/mastercard-antom-agent-pay-singapur/)
- [Stripe agentic commerce docs](https://docs.stripe.com/agentic-commerce) - Stripe's documentation for selling through AI agents.
- [Adyen agentic commerce docs](https://docs.adyen.com/online-payments/agentic-commerce) - Adyen's documentation for payments initiated by AI agents. [Analysis](https://www.agentic-commerce.sh/en/news/adyen-agentic-klarna-checkout/)
- [PayPal Agentic Commerce Services](https://developer.paypal.com/agentic-commerce-services/about) - PayPal's developer services for agentic commerce. [Analysis](https://www.agentic-commerce.sh/en/news/paypal-agentic-virtual-card/)
- [Lightspark Agent Accounts](https://www.lightspark.com/news/lightspark/introducing-lightspark-agent-accounts) - Payment accounts that an AI agent can hold and spend from. [Analysis](https://www.agentic-commerce.sh/en/news/lightspark-agent-accounts/)
- [AWS Marketplace agentic payments](https://aws.amazon.com/about-aws/whats-new/2026/11/marketplace-agentic-payments-agentcore/) - Pay-per-request purchases by agents with x402 and AgentCore. [Analysis](https://www.agentic-commerce.sh/en/news/aws-marketplace-agentcore-x402/)

## Agent identity and verification

How a merchant recognises a legitimate shopping agent. Background in the [Web Bot Auth guide](https://www.agentic-commerce.sh/en/guides/tell-shopping-agents-from-bots/).

- [IETF Web Bot Auth working group](https://datatracker.ietf.org/wg/webbotauth/about/) - Standardises how bots and agents authenticate to websites.
- [RFC 9421 · HTTP Message Signatures](https://www.rfc-editor.org/rfc/rfc9421) - The signature mechanism that Web Bot Auth builds on.
- [Cloudflare signed agents](https://developers.cloudflare.com/bots/concepts/bot/signed-agents/) - How signed agents are verified at the network edge.
- [Cloudflare · Securing agentic commerce](https://blog.cloudflare.com/secure-agentic-commerce) - Agent verification together with Visa and Mastercard.

## Shopping agents and assistants

Consumer and business agents that search, compare and buy. Each entry links the announcement and an analysis for merchants.

- [ChatGPT Wallet](https://openai.com/index/introducing-chatgpt-wallet/) - OpenAI connects the conversation to payment and checkout. [Analysis](https://www.agentic-commerce.sh/en/news/chatgpt-wallet-agentenzahlung/)
- [ChatGPT Business Hub](https://openai.com/index/introducing-businesses-chatgpt/) - Business agents inside ChatGPT. [Analysis](https://www.agentic-commerce.sh/en/news/openai-business-hub-agenten/)
- [Gemini Tasks with Google Pay](https://blog.google/innovation-and-ai/products/gemini-app/tasks-in-gemini-free-new-features/) - Gemini can complete purchases with Google Pay in the US. [Analysis](https://www.agentic-commerce.sh/en/news/gemini-tasks-google-pay-einkauf/)
- [Google Wallet in AI Mode](https://blog.google/products-and-platforms/products/search/google-search-personal-intelligence-apps/) - Spending context from Google Wallet in AI Mode in Search. [Analysis](https://www.agentic-commerce.sh/en/news/google-wallet-personal-intelligence/)
- [Alexa for Shopping](https://www.aboutamazon.com/news/retail/alexa-for-shopping-text-to-shop) - Shopping by text message with Alexa. [Analysis](https://www.agentic-commerce.sh/en/news/alexa-text/)
- [Meta Muse](https://about.fb.com/news/2026/11/meta-welcomes-loblaw-as-first-canadian-retail-partner-to-muse/) - Meta's assistant from meal planning to grocery checkout. [Analysis](https://www.agentic-commerce.sh/en/news/meta-muse-loblaw-lebensmittel/)
- [Poppy by Sierra](https://sierra.ai/uk/blog/releasing-poppy) - Personal agents that work with businesses through the Personal Agent Protocol. [Analysis](https://www.agentic-commerce.sh/en/news/poppy-personal-agent-protocol-1-0/)
- [Klarna AI assistant](https://investors.klarna.com/News--Events/news/news-details/2026/From-returns-to-restaurant-bookings-Klarnas-AI-assistant-finds-the-best-product--price-buys-it-for-you-and-you-dont-pay-until-it-arrives-2026-AsJ__j3bx3/default.aspx) - An assistant that finds, buys and pays in WhatsApp and iMessage. [Analysis](https://www.agentic-commerce.sh/en/news/klarna-ki-assistent-whatsapp-imessage/)
- [mate](https://www.einnews.com/pr_news/955148658/mate-launches-text-based-ai-shopping-agent-ahead-of-black-friday) - A shopping agent inside the messaging thread. [Analysis](https://www.agentic-commerce.sh/en/news/mate-shopping-agent-chat/)
- [Squaremates](https://squareup.com/us/en/press/introducing-squaremates) - Square's agent for work across a seller's business. [Analysis](https://www.agentic-commerce.sh/en/news/square-squaremates-haendler-agent/)

## Open source experiments

Experimental prototypes and tools from the [Shopware Agentic Commerce Lab](https://github.com/agentic-commerce-lab), open source under their own licences.

- [Agentic Resource Discovery](https://github.com/agentic-commerce-lab/agentic-resource-discovery-plugin) - Help an agent understand what a shop offers and how to work with it. The plugin publishes a directory of data, services and available actions.
- [Agentic Experience Protocol](https://github.com/agentic-commerce-lab/AXP-protocol) - A product is more than a name and a price. AXP brings variants, configurations, quality signals and embedded experiences into an agent’s interface.
- [WebMCP for Shopware](https://github.com/agentic-commerce-lab/webmcp-plugin) - Search products, select variants and work with the cart: the shop exposes these capabilities inside the current browser session.
- [Bright Shelf](https://getbrightshelf.com/) - Drafts product imagery, ads and short videos. The shop URL provides context about the brand and its tone.
- [Commerce Client SDK](https://github.com/agentic-commerce-lab/commerce-client-sdk/releases/tag/v0.1.0) - REST clients in TypeScript and Python for UCP discovery, carts and checkout.
- [Shopping Assistant Starter Kit](https://github.com/agentic-commerce-lab/shopping-assistant-starter-kit) - A shopping assistant in the merchant’s own shop: customers can ask questions, compare products and add suitable items to their cart.
- [Sales Agent Harness](https://github.com/agentic-commerce-lab/sales-agent-harness) - A sales agent needs reliable rules. This framework connects advice, product search and cart preparation to the merchant’s policies and systems.
- [Shopware as an MCP App](https://github.com/agentic-commerce-lab/swag-mcp-app) - Bring the catalogue into the assistant: customers search for items, see product cards and prepare their cart in a conversation.
- [A2UI for Shopware Frontends](https://github.com/agentic-commerce-lab/SwagA2UI) - What does a shop look like when its interface responds to the customer’s current intention? This experiment lets an agent generate relevant views and render them in the browser.
- [Page Agent Bridge](https://github.com/agentic-commerce-lab/PageAgentShopwareBridge) - A customer describes what they want to do. An agent panel can read the shop page and carry out steps through its interface.
- [Merchant Quote Agent](https://github.com/agentic-commerce-lab/merchant-quote-agent-plugin) - A B2B customer asks for a better price. The Quote Agent responds within the discount limits set by the merchant.
- [Shopware × Claude Commerce](https://github.com/agentic-commerce-lab/shopware-claude-commerce) - Two perspectives on the same business: a shopping agent finds products and prepares a purchase. A merchant agent reviews sales and proposes changes.
- [x402 Payments](https://github.com/agentic-commerce-lab/x402-payment-plugin) - How does an automated buyer pay? This project explores a payment flow in which the shop sends a payment request and the buyer signs it digitally.
- [Newsatoshi Commons (Private x402 + PayWords + nsUSD)](https://github.com/theguysaccount/newsatoshi-commons) - Rust HTTP 402 and MCP gateway (`PolyForm-Noncommercial-1.0.0`) pairing `x402 v2` Base/Arbitrum/Polygon USDC with zero-gas `O(1)` SHA-256 PayWord micropayment channels (`RFC-0022`), a 60-second Express/Next.js/FastAPI/Axum paywall generator, and RFC-0028 `nsUSD` shielded dollar accounting. [Live Gateway](https://commons.newsatoshi.org/nsusd)
- [Pawl](https://github.com/agentic-commerce-lab/pawl) - Agents can write a great deal of code. Pawl connects requirements to verifiable outcomes and records which work actually passes a check.
- [Agent in a Box](https://github.com/agentic-commerce-lab/agent-in-a-box) - A workspace for the coding agent: tools and runtime live in a development environment dedicated to the project.
- [RFQ Bench](https://github.com/agentic-commerce-lab/rfq-bench) - Which agent negotiates better, and at what cost? RFQ Bench compares buyers, sellers and strategies in controlled B2B negotiations.
- [Lightcone](https://github.com/agentic-commerce-lab/lightcone-webmcp-game) - A game of hide-and-seek with an agent that sees very little of its surroundings. It needs to use tools and adapt its search during play.

## Research, benchmarks and data

Studies and measurements with a public source. More figures with dates in [agentic commerce statistics](https://www.agentic-commerce.sh/en/guides/agentic-commerce-statistics/).

- [Visa AI shopping benchmark](https://visa.gcs-web.com/news-releases/news-release-details/visa-releases-first-its-kind-industry-benchmark-ai-shopping) - 22 models tested across 15 shopping scenarios. [Analysis](https://www.agentic-commerce.sh/en/news/visa-benchmark/)
- [a16z · Welcome to the B2A economy](https://a16z.com/welcome-to-the-b2a-economy-how-agents-buy/) - How shopping agents choose what to buy and where. [Analysis](https://www.agentic-commerce.sh/en/news/a16z-test-einkaufsagenten-haendlerwahl/)
- [McKinsey · Who wins when AI does the shopping?](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/who-wins-when-ai-does-the-shopping-new-evidence-on-agentic-commerce) - New evidence on how agents shift purchasing.
- [G2 · Merchant readiness for agentic commerce](https://research-hub.g2.com/merchant-readiness-for-agentic-commerce) - Can merchants identify agent orders? [Analysis](https://www.agentic-commerce.sh/en/news/g2-studie-agentenbestellungen-erkennen/)
- [i22 · Agentic commerce readiness study](https://i22.ai/agentic-commerce-readiness-studie) - How far an AI agent gets in 48 German online shops. [Analysis](https://www.agentic-commerce.sh/en/news/i22-studie-agentic-commerce-deutschland/)
- [Forter · AI agent order data](https://www.forter.com/blog/ai-agent-order-data/) - What early agent orders show about checkout and fraud. [Analysis](https://www.agentic-commerce.sh/en/news/forter-orders/)
- [DHL eCommerce · AI price comparison survey](https://group.dhl.com/en/media-relations/press-releases/2026/nearly-nine-in-ten-shoppers-use-or-plan-to-use-ai-to-find-the-best-price.html) - Nearly nine in ten shoppers use or plan to use AI to find the best price. [Analysis](https://www.agentic-commerce.sh/en/news/black-friday-2026-ki-preisvergleich/)
- [Gartner · CMOs and brand information in AI](https://www.gartner.com/en/newsroom/press-releases/2026-11-09-gartner-survey-finds-42-percent-of-cmos-are-monitoring-brand-misinformation-in-ai-generated-content) - How marketing teams monitor what AI says about their brand. [Analysis](https://www.agentic-commerce.sh/en/news/gartner-ki-markeninformationen/)

## Tools for merchants

Vendor-neutral checks a merchant can run before talking to providers.

- [Agentic Commerce Readiness Scanner](https://scanner.agentic-commerce.org/) - 32 public checks in 8 categories: what agents can read on a shop's website.
- [UCP conformance tests](https://github.com/Universal-Commerce-Protocol/conformance) - Check a UCP endpoint against the specification.
- [Purchase acceptance test](https://www.agentic-commerce.sh/en/guides/testing-agent-purchases/) - Test scenarios for agent purchases, from approval to order.

## Standards bodies and communities

Where the open standards behind agentic commerce are developed.

- [Agentic Commerce Alliance](https://www.agentic-commerce.org/) - Independent, non-profit alliance of merchants, platforms, payment providers and integrators.
- [Agentic AI Foundation](https://aaif.io/) - Linux Foundation home for open agent standards, including MCP.
- [W3C Web Machine Learning Community Group](https://www.w3.org/community/webmachinelearning/) - Incubates WebMCP, structured tools for agents in the browser.
- [IETF Web Bot Auth](https://datatracker.ietf.org/wg/webbotauth/about/) - Working group for agent and bot authentication.
- [x402 Foundation](https://github.com/x402-foundation) - Governance and working groups for x402, including identity and card acceptance.
- [FIDO Alliance](https://fidoalliance.org/) - Standardisation work to which AP2 has been contributed.

## Recent developments

Announcements from the last weeks, each with the original source and a short analysis for merchants.

- **2026-11-26** · [Mastercard and Debia plan agent shopping pilots through to pickup](https://www.prnewswire.com/apac/news-releases/debia-and-mastercard-sign-mou-to-advance-agentic-commerce-302950485.html) · [Analysis](https://www.agentic-commerce.sh/en/news/mastercard-debia-agent-pay-piloten/)
- **2026-11-25** · [Forter tracks agent orders through store pages and commerce protocols](https://ai.forter.com/agentic-bfcm) · [Analysis](https://www.agentic-commerce.sh/en/news/forter-agentenbestellungen-checkout-wege/)
- **2026-11-25** · [Shopware checks payment options before UCP checkout completion](https://github.com/shopware/agentic-commerce/pull/380) · [Analysis](https://www.agentic-commerce.sh/en/news/shopware-ucp-checkout-zahlungsarten/)
- **2026-11-25** · [An agent in ChatGPT buys biscotti and pays with Bitcoin](https://www.globenewswire.com/news-release/2026/11/25/3410633/0/en/agnic-ai-and-gobtc-pay-bring-bitcoin-to-ai-agent-checkout-with-a-live-mainnet-purchase-in-chatgpt.html) · [Analysis](https://www.agentic-commerce.sh/en/news/agnic-bitcoin-biscotti-chatgpt/)
- **2026-11-24** · [Meta Muse can put together a weekly shop at Sainsbury’s](https://corporate.sainsburys.co.uk/news/press-releases/muse-from-meta-gives-customers-even-more-choice-in-how-they-shop-with-sainsbury-s/) · [Analysis](https://www.agentic-commerce.sh/en/news/meta-muse-sainsburys-wocheneinkauf/)
- **2026-11-24** · [Wells Fargo sets terms for third party AI agents in online banking](https://www.wellsfargo.com/online-banking/online-access-agreement/) · [Analysis](https://www.agentic-commerce.sh/en/news/wells-fargo-ki-agenten-onlinebanking/)
- **2026-11-23** · [Meta Muse can shop through Walmart’s Agent Gateway](https://www.walmart.com/cp/walmart-agent-gateway/1280482) · [Analysis](https://www.agentic-commerce.sh/en/news/walmart-muse-agent-gateway/)
- **2026-11-23** · [How shopping agents choose what to buy and where to buy it](https://a16z.com/welcome-to-the-b2a-economy-how-agents-buy/) · [Analysis](https://www.agentic-commerce.sh/en/news/a16z-test-einkaufsagenten-haendlerwahl/)
- **2026-11-23** · [PayPal sets refund and seller protection terms for agentic virtual cards](https://www.paypalobjects.com/marketing/ua/OA/agentic-commerce-merchant-vc-tnc/en-US-112326.pdf) · [Analysis](https://www.agentic-commerce.sh/en/news/paypal-agentic-virtual-card/)
- **2026-11-23** · [Google Wallet brings spending context to AI Mode in Search](https://blog.google/products-and-platforms/products/search/google-search-personal-intelligence-apps/) · [Analysis](https://www.agentic-commerce.sh/en/news/google-wallet-personal-intelligence/)
- **2026-11-20** · [How far can AI agents get in German online shops?](https://i22.ai/agentic-commerce-readiness-studie) · [Analysis](https://www.agentic-commerce.sh/en/news/i22-studie-agentic-commerce-deutschland/)
- **2026-11-20** · [Black Friday 2026: What AI price comparisons need to see](https://group.dhl.com/en/media-relations/press-releases/2026/nearly-nine-in-ten-shoppers-use-or-plan-to-use-ai-to-find-the-best-price.html) · [Analysis](https://www.agentic-commerce.sh/en/news/black-friday-2026-ki-preisvergleich/)
- **2026-11-20** · [Stripe’s Link Agent Wallet data puts travel first by spend](https://x.com/ernietedeschi/article/2123852064027471901) · [Analysis](https://www.agentic-commerce.sh/en/news/stripe-link-agent-wallet-ausgaben-reisen/)
- **2026-11-20** · [Klarna joins Adyen Agentic checkout](https://investors.klarna.com/News--Events/news/news-details/2026/Adyen-Merchants-Can-Now-Offer-Klarna-in-AI-Agent-Checkout/default.aspx) · [Analysis](https://www.agentic-commerce.sh/en/news/adyen-agentic-klarna-checkout/)
- **2026-11-19** · [AWS Marketplace x402 payments: How AI agents buy a single request](https://aws.amazon.com/about-aws/whats-new/2026/11/marketplace-agentic-payments-agentcore/) · [Analysis](https://www.agentic-commerce.sh/en/news/aws-marketplace-agentcore-x402/)
- **2026-11-19** · [Walmart reports 129% growth in Sparky usage](https://stock.walmart.com/_assets/_6eff40d47b6de9e4a6d86158aa985c07/walmart/db/938/10001/transcript_management_call/Earnings_Transcript_%28FY27_Q3%29.pdf) · [Analysis](https://www.agentic-commerce.sh/en/news/walmart-sparky-warenkorb/)
- **2026-11-19** · [Mastercard and Antom test what AI agents can pay for](https://www.ant-intl.com/en/news/detail/mastercard-and-ant-international-advance-trusted-agentic-commerce-in-asia-pacific/) · [Analysis](https://www.agentic-commerce.sh/en/news/mastercard-antom-agent-pay-singapur/)
- **2026-11-19** · [G2 study: Can merchants identify agent orders?](https://research-hub.g2.com/merchant-readiness-for-agentic-commerce) · [Analysis](https://www.agentic-commerce.sh/en/news/g2-studie-agentenbestellungen-erkennen/)
- **2026-11-18** · [Visa Agentic Ready: Payment providers prepare merchants for AI agents](https://www.mynewsdesk.com/uk/visa/pressreleases/visa-expands-agentic-ready-to-help-scale-trusted-ai-commerce-across-europe-3478924) · [Analysis](https://www.agentic-commerce.sh/en/news/visa-agentic-ready-akzeptanz/)
- **2026-11-18** · [Meta Muse and Loblaw: From meal planning to grocery checkout](https://about.fb.com/news/2026/11/meta-welcomes-loblaw-as-first-canadian-retail-partner-to-muse/) · [Analysis](https://www.agentic-commerce.sh/en/news/meta-muse-loblaw-lebensmittel/)
- **2026-11-18** · [Shopware 6.7.16.1 validates custom MCP tool responses](https://developer.shopware.com/release-notes/6.7/6.7.16.1.html) · [Analysis](https://www.agentic-commerce.sh/en/news/shopware-6-7-16-1-mcp/)
- **2026-11-17** · [Razorpay and Meta connect shopping advice and payment in WhatsApp](https://razorpay.com/newsroom/razorpay-goes-live-on-meta-business-agent-enabling-payments-inside-whatsapp-business-app/) · [Analysis](https://www.agentic-commerce.sh/en/news/razorpay-meta-whatsapp/)
- **2026-11-17** · [Lightspark Agent Accounts: A payment account for AI agents](https://www.lightspark.com/news/lightspark/introducing-lightspark-agent-accounts) · [Analysis](https://www.agentic-commerce.sh/en/news/lightspark-agent-accounts/)
- **2026-11-17** · [Klarna tests AI shopping in WhatsApp and iMessage](https://investors.klarna.com/News--Events/news/news-details/2026/From-returns-to-restaurant-bookings-Klarnas-AI-assistant-finds-the-best-product--price-buys-it-for-you-and-you-dont-pay-until-it-arrives-2026-AsJ__j3bx3/default.aspx) · [Analysis](https://www.agentic-commerce.sh/en/news/klarna-ki-assistent-whatsapp-imessage/)
- **2026-11-17** · [Gemini Tasks can shop with Google Pay in the US](https://blog.google/innovation-and-ai/products/gemini-app/tasks-in-gemini-free-new-features/) · [Analysis](https://www.agentic-commerce.sh/en/news/gemini-tasks-google-pay-einkauf/)
- **2026-11-13** · [Amazon is considering a global product index for AI search, Reuters reports](https://kelo.com/2026/11/13/exclusive-amazons-plan-to-own-the-worlds-product-data-and-fight-ai-shopping-agents/) · [Analysis](https://www.agentic-commerce.sh/en/news/amazon-world-product-graph/)
- **2026-11-13** · [ChatGPT Wallet and Business Hub: How OpenAI connects the conversation to the purchase](https://openai.com/index/introducing-chatgpt-wallet/) · [Analysis](https://www.agentic-commerce.sh/en/news/chatgpt-wallet-agentenzahlung/)
- **2026-11-13** · [Poppy 1.0: How personal agents work with businesses](https://sierra.ai/uk/blog/releasing-poppy) · [Analysis](https://www.agentic-commerce.sh/en/news/poppy-personal-agent-protocol-1-0/)
- **2026-11-12** · [Replit gives its agent business shopping and advertising tasks](https://replit.com/blog/replit-agent-ads-commerce) · [Analysis](https://www.agentic-commerce.sh/en/news/replit-agent-einkauf-werbung/)
- **2026-11-12** · [Squaremates: An agent takes on work across a merchant’s business](https://squareup.com/us/en/press/introducing-squaremates) · [Analysis](https://www.agentic-commerce.sh/en/news/square-squaremates-haendler-agent/)
- **2026-11-12** · [J.Crew and Claude: A shopping assistant puts complete outfits together](https://claude.com/resources/articles/j-crew-style-advisor-with-claude) · [Analysis](https://www.agentic-commerce.sh/en/news/jcrew-style-advisor-claude/)
- **2026-11-11** · [Digital Fairness Act: What the EU proposal means for shopping agents and merchants](https://commission.europa.eu/document/download/0575d59f-554f-4a9e-b54b-e6b717175809_en?filename=Proposal+for+a+Digital+Fairness+Act_0.pdf) · [Analysis](https://www.agentic-commerce.sh/en/news/digital-fairness-act-einkaufsagenten/)
- **2026-11-10** · [The End of Software as We Know It](https://www.linkedin.com/pulse/end-software-we-know-stefan-hamann-z81he/) · [Analysis](https://www.agentic-commerce.sh/en/news/holodeck/)
- **2026-11-10** · [mate brings a shopping agent into the messaging thread](https://www.einnews.com/pr_news/955148658/mate-launches-text-based-ai-shopping-agent-ahead-of-black-friday) · [Analysis](https://www.agentic-commerce.sh/en/news/mate-shopping-agent-chat/)
- **2026-11-10** · [ChatGPT Business Hub: Business Agents expand beyond the US](https://openai.com/index/introducing-businesses-chatgpt/) · [Analysis](https://www.agentic-commerce.sh/en/news/openai-business-hub-agenten/)
- **2026-11-09** · [What AI says about a brand: Gartner examines how marketing teams respond](https://www.gartner.com/en/newsroom/press-releases/2026-11-09-gartner-survey-finds-42-percent-of-cmos-are-monitoring-brand-misinformation-in-ai-generated-content) · [Analysis](https://www.agentic-commerce.sh/en/news/gartner-ki-markeninformationen/)
- **2026-11-06** · [Shopping by message: Alexa for Shopping moves into the chat](https://www.aboutamazon.com/news/retail/alexa-for-shopping-text-to-shop) · [Analysis](https://www.agentic-commerce.sh/en/news/alexa-text/)
- **2026-11-05** · [When the shopping agent buys anyway: What Visa’s test shows](https://visa.gcs-web.com/news-releases/news-release-details/visa-releases-first-its-kind-industry-benchmark-ai-shopping) · [Analysis](https://www.agentic-commerce.sh/en/news/visa-benchmark/)
- **2026-11-04** · [Amazon Shop Direct opens a new route for independent merchants](https://www.aboutamazon.com/news/retail/amazon-shop-direct-merchant-workspace) · [Analysis](https://www.agentic-commerce.sh/en/news/amazon-shop-direct/)
- **2026-11-04** · [Google brings UCP checkout to Canada](https://blog.google/intl/en-ca/products/explore-get-answers/a-new-way-to-shop-introducing-a-more-intuitive-agentic-shopping-experience-for-consumers-and-retailers-in-canada/) · [Analysis](https://www.agentic-commerce.sh/en/news/google-ucp-canada/)
- **2026-11-03** · [Zalando Extended: Zalando’s agent will shop at Westwing from 2027](https://www.webdisclosure.com/press-release/zalando-se-etr-de000zal-zalando-grows-profitably-in-q3-driven-by-very-strong-b2b-expansion-and-continues-innovating-through-ai-with-zalando-extended-huj09XBfJfh) · [Analysis](https://www.agentic-commerce.sh/en/news/zalando-extended-westwing-agent/)
- **2026-11-02** · [Bright Shelf: How Shopware’s lab is exploring AI product visuals](https://www.shopware.com/en/news/shopware-6-release-news-november-2026/) · [Analysis](https://www.agentic-commerce.sh/en/news/bright-shelf/)
- **2026-11-02** · [What early agent orders tell us about checkout](https://www.forter.com/blog/ai-agent-order-data/) · [Analysis](https://www.agentic-commerce.sh/en/news/forter-orders/)

## Books and long reads

- [Agentic Commerce: The Handbook for Commerce Strategy, Technology and Leadership](https://www.agentic-commerce.sh/book/en/) - Stefan Hamann, 2026. Free online in English and German.
- [Agentic Commerce: Protocols, Standards, and Reference Architectures](https://www.agentic-commerce.sh/library/developers-2026/) - Developer whitepaper, January 2026.
- [Agentic Commerce: How AI Autonomy Will Redefine Ecommerce Competition](https://www.agentic-commerce.sh/library/whitepaper-2025/) - Whitepaper, January 2025.

## Related lists

- [Merit-Systems/awesome-agentic-commerce](https://github.com/Merit-Systems/awesome-agentic-commerce) - x402 and crypto payment rails.
- [xpaysh/awesome-agentic-commerce](https://github.com/xpaysh/awesome-agentic-commerce) - Protocols and platform plugins.
- [bitrefill/awesome-agentic-payments](https://github.com/bitrefill/awesome-agentic-payments) - Agent payment protocols and rails.
- [Upsonic/awesome-ucp](https://github.com/Upsonic/awesome-ucp) - UCP resources.
- [yifeizhangcs/awesome-agentic-commerce](https://github.com/yifeizhangcs/awesome-agentic-commerce) - Research papers along the commerce pipeline.

## Contributing

Suggestions are welcome as issues or pull requests. A protocol needs a public specification and a named publisher. An implementation needs public source code. Shop systems and e-commerce platforms are out of scope. Please link the primary source, not a summary of it. Protocol data is maintained in one place and regenerated, so a pull request may be applied to the source data instead of merged directly.

## Licence

[CC0 1.0](LICENSE). Maintained by [Stefan Hamann](https://stefan-hamann.de/).
