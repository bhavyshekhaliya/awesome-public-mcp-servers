# Awesome Public MCP Servers

<p align="center">
  <strong>Public MCP servers, organized around what you want to connect.</strong>
</p>

<p align="center">
  <a href="https://awesome.re"><img alt="Awesome" src="https://awesome.re/badge.svg"></a>
  <img alt="Model Context Protocol" src="https://img.shields.io/badge/MCP-servers-13795b">
  <a href="LICENSE"><img alt="CC0 1.0 license" src="https://img.shields.io/badge/license-CC0%201.0-555555"></a>
</p>

Discover MCP servers that connect assistants and agents to useful tools, data,
and workflows. Every entry should link to an official connection page,
endpoint, or public source repository and provide enough context to evaluate
how the server works before connecting.

Created and maintained by [0mcp.io](https://0mcp.io).

> This directory is being built. Contributions are welcome; please read
> [CONTRIBUTING.md](CONTRIBUTING.md) before adding a server.

## Contents

- [Categories](#categories)
- [Servers](#servers)
- [Legend](#legend)
- [Contributing](#contributing)
- [Maintainer](#maintainer)

## Categories

Categories are ordered from everyday and personal workflows to technical
infrastructure. Choose the category that best describes the primary job a
server helps someone complete; tags are supporting labels, not a second
category system.

| Category | Includes |
| --- | --- |
| Personal Organization | Calendars, tasks, notes, boards, and personal planning |
| Communication | Email, chat, meetings, and customer conversations |
| Travel and Location | Places, maps, weather, geocoding, and routing |
| Finance and Commerce | Payments, invoicing, markets, shopping, and commerce |
| Home and Lifestyle | Smart-home devices, scenes, and household context |
| Files and Storage | Documents, object storage, content management, and file systems |
| Design and Creative | Visual design, whiteboards, graphics, and content creation |
| Work and Productivity | Work planning, project management, CRM, and business workflows |
| Media and Content | Audio, speech, voice, and other creative media |
| Search and Research | Web search, knowledge bases, retrieval, and citations |
| Browser and Automation | Browsing, scraping, testing, and workflow automation |
| AI and LLM | Model providers, inference, evaluation, and agent tooling |
| Data and Databases | SQL, search, vector stores, analytics, and data platforms |
| Developer Tools | Code hosting, repositories, CI/CD, packages, and APIs |
| Cloud and Infrastructure | Hosting, deployment, and infrastructure |
| Monitoring and Security | Security analysis, incident response, and operational tooling |
| Science and Computation | Mathematical computation, scientific knowledge, and symbolic tools |

## Servers

These entries are hosted or publicly installable MCP servers published and
maintained by the linked providers. Check each provider's documentation for
plan requirements, permissions, rate limits, and data-handling terms before
connecting.

### Personal Organization

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Google Calendar | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://calendarmcp.googleapis.com/mcp/v1`, HTTP) | List calendars and events, create/update/delete events, respond to invitations, and suggest times | Google Cloud project with Calendar API and Calendar MCP API enabled; OAuth 2.0; Developer Preview | `official` `calendar` `planning` |
| Notion | [Connection guide](https://developers.notion.com/guides/mcp/get-started-with-mcp) (`https://mcp.notion.com/mcp`) | Workspace search, pages, and content management | Notion account (OAuth) | `official` `knowledge-base` `documents` |
| Todoist | [Official source repository](https://github.com/Doist/todoist-mcp) (hosted `https://ai.todoist.net/mcp`, Streamable HTTP; local `npx @doist/todoist-mcp`, stdio) | Read, create, and update tasks and projects for personal planning workflows | Todoist OAuth on the hosted server or Todoist API key for local use | `official` `tasks` `planning` |
| Trello | [Trello MCP guide](https://support.atlassian.com/trello/docs/connect-trello-to-ai-assistants-with-trello-mcp/) (`https://mcp.trello.com/v1`, HTTP) | Search boards and cards; create, update, move, archive, and complete cards; manage lists and checklists | Trello account and OAuth 2.0; one workspace per connection; available on all plans | `official` `boards` `tasks` |

### Communication

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Google Chat | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://chatmcp.googleapis.com/mcp/v1`, HTTP) | Search conversations and messages, list messages, and send messages | Google Cloud project with Chat API/MCP API and a Chat app configured; OAuth 2.0; Developer Preview | `official` `messaging` `everyday` |
| Gmail | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://gmailmcp.googleapis.com/mcp/v1`, HTTP) | Search email threads, read messages, manage labels, and create drafts | Google Cloud project with Gmail API and Gmail MCP API enabled; OAuth 2.0; Developer Preview | `official` `email` `office` |
| Intercom | [MCP guide](https://developers.intercom.com/docs/guides/mcp) (`https://mcp.intercom.com/mcp`) | Conversations, contacts, companies, users, and Help Center articles | Intercom OAuth or bearer token; US-hosted workspaces | `official` `customer-support` `conversations` |
| Slack | [MCP server overview](https://docs.slack.dev/ai/slack-mcp-server/) (`https://mcp.slack.com/mcp`) | Search messages, files, users, and channels; read and send messages; manage canvases and reactions | Slack OAuth with a registered app | `official` `messaging` `collaboration` |

### Travel and Location

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Google Maps Grounding Lite | [MCP documentation](https://developers.google.com/maps/ai/grounding-lite) (`https://mapstools.googleapis.com/mcp`, Streamable HTTP) | Search places, look up current and forecast weather, and compute walking or driving route distance and duration | Google Maps API key or OAuth; Google Cloud project and billing setup required | `official` `maps` `routing` |
| Mapbox | [MCP server documentation](https://docs.mapbox.com/api/guides/mcp-server/) (`https://mcp.mapbox.com/mcp`, Streamable HTTP) | Directions, isochrones, address and point-of-interest lookup, reverse geocoding, static maps, and geospatial resources | Mapbox OAuth for the hosted server or an access token for local deployment | `official` `geocoding` `navigation` |

### Finance and Commerce

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| AgentServices | [MCP details](https://agentservices.to) (`https://api.agentservices.to/mcp`) | x402-paid crypto and market data APIs - BTC indicators, DeFi stats, macro data, exchange analytics, 54 services, and 37 MCP tools | No API key; x402 USDC payment for paid tools | `official` `market-data` `crypto` |
| BuyWhere | [MCP server documentation](https://api.buywhere.ai) (`https://api.buywhere.ai/mcp`) | Product search, merchant comparison, and real-time pricing data across 9 Asian and US markets | API key (free tier available) | `community` `shopping` `commerce` |
| Klaviyo | [MCP server documentation](https://developers.klaviyo.com/en/docs/klaviyo_mcp_server) (`https://mcp.klaviyo.com/mcp`) | Campaigns, flows, performance reports, templates, and Klaviyo account data | Klaviyo OAuth; Owner, Admin, or Manager role required | `official` `marketing` `campaigns` |
| PayPal | [MCP server announcement](https://developer.paypal.com/community/blog/paypal-model-context-protocol/) ([MCP portal](https://mcp.paypal.com)) | Create and manage invoices and invoice links; the official toolkit also supports orders, refunds, subscriptions, disputes, and tracking | PayPal developer credentials and access token; production use requires a PayPal Business account | `official` `payments` `invoicing` |
| Shopify Storefront MCP | [Storefront MCP server documentation](https://shopify.dev/docs/apps/build/storefront-mcp/servers/storefront) (`https://{shop}.myshopify.com/api/mcp`) | Store catalogs, product search, policies, carts, and storefront commerce flows; UCP catalog tools use `/api/ucp/mcp` | None for Storefront MCP/cart endpoints; checkout and customer-account flows may require auth | `official` `commerce` `shopping` |
| Square | [MCP server documentation](https://developer.squareup.com/docs/mcp) ([official source repository](https://github.com/square/square-mcp-server)) (`https://mcp.squareup.com/sse`, SSE) | Natural-language access to Square seller and commerce operations, including customers, orders, and items | Square account and OAuth with granular scopes; production access reaches live seller resources, so Sandbox testing is recommended; Beta | `official` `payments` `commerce` |
| Stripe | [MCP documentation](https://docs.stripe.com/mcp) (`https://mcp.stripe.com/`) | Payments, billing, products, customers, and Stripe documentation | Stripe OAuth or restricted API key | `official` `payments` `billing` |
| Xero | [Xero AI toolkit](https://developer.xero.com/ai) ([official source repository](https://github.com/XeroAPI/xero-mcp-server)) (`npx -y @xeroapi/xero-mcp-server@latest`, stdio) | Contacts, accounts, invoices, credit notes, payments, quotes, bank transactions, reports, and tracking categories | Xero organization and developer API credentials; OAuth 2 custom connection or bearer token; a demo company is recommended for testing | `official` `accounting` `invoicing` |

### Home and Lifestyle

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Home Assistant | [MCP server integration](https://www.home-assistant.io/integrations/mcp_server/) (`https://<your_home_assistant_external_url>/api/mcp`, Streamable HTTP) | Read real-time entity context and control the home devices and entities exposed by the user | Home Assistant instance with the MCP integration; OAuth or long-lived access token; a public URL is required for cloud connectors | `official` `smart-home` `home-automation` |

### Files and Storage

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Box | [MCP server guide](https://developer.box.com/guides/box-mcp) (`https://mcp.box.com`) | Files, folders, search, collaboration, Box AI queries, hubs, and document generation | Box OAuth; admin enablement may be required | `official` `documents` `enterprise` |
| Dropbox | [Remote MCP setup](https://help.dropbox.com/integrations/connect-dropbox-mcp-server) (`https://mcp.dropbox.com/mcp`) | File and folder search, content extraction, file creation, sharing, revisions, restore, and transcription | Dropbox OAuth; custom clients need app credentials | `official` `files` `storage` |
| Google Docs | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://docsmcp.googleapis.com/mcp/v1`, HTTP) | Read and update Google Docs content | Google Cloud project with Docs API and Docs MCP API enabled; OAuth 2.0; Developer Preview | `official` `documents` `office` |
| Google Drive | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://drivemcp.googleapis.com/mcp/v1`, HTTP) | Search, read, create, copy, and download files; inspect metadata and permissions | Google Cloud project with Drive API and Drive MCP API enabled; OAuth 2.0; Developer Preview | `official` `files` `workspace` |
| Google Sheets | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://sheetsmcp.googleapis.com/mcp/v1`, HTTP) | Read and update spreadsheet values, formulas, dimensions, and workbook structure | Google Cloud project with Sheets API and Sheets MCP API enabled; OAuth 2.0; Developer Preview | `official` `spreadsheets` `office` |
| Google Slides | [Google Workspace MCP server documentation](https://developers.google.com/workspace/guides/configure-mcp-servers?hl=en) (`https://slidesmcp.googleapis.com/mcp/v1`, HTTP) | Read and update presentation content and layout | Google Cloud project with Slides API and Slides MCP API enabled; OAuth 2.0; Developer Preview | `official` `presentations` `office` |

### Design and Creative

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Canva | [MCP documentation](https://www.canva.dev/docs/mcp/) (`https://mcp.canva.com/mcp`) | Design creation and editing, asset and brand management, library search, exports, and comments | Canva OAuth (per-user) | `official` `design` `assets` |
| Figma | [Remote server setup](https://developers.figma.com/docs/figma-mcp-server/remote-server-installation/) (`https://mcp.figma.com/mcp`) | Design context, code generation, canvas editing, and FigJam | Figma account (OAuth) | `official` `design` `figjam` |
| Miro | [MCP server documentation](https://developers.miro.com/docs/miro-mcp) (`https://mcp.miro.com/`) | Search and summarize boards, create diagrams, and add board content such as frames, cards, shapes, and tables | Miro OAuth | `official` `whiteboards` `collaboration` |
| Webflow | [MCP server documentation](https://developers.webflow.com/mcp/reference/how-it-works) (`https://mcp.webflow.com/mcp`) | Site authoring, CMS content, styles, components, variables, pages, assets, and Designer context | Webflow OAuth; the Bridge App is required for live Designer capabilities | `official` `website-builder` `design` |

### Work and Productivity

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Asana | [MCP integration guide](https://developers.asana.com/docs/integrating-with-asanas-mcp-server) (`https://mcp.asana.com/v2/mcp`) | Work graph, tasks, projects, and planning workflows | Asana OAuth 2.0 (MCP app) | `official` `project-management` `tasks` |
| Atlassian Rovo | [Rovo MCP overview](https://developer.atlassian.com/cloud/rovo-mcp/) (`https://mcp.atlassian.com/v1/mcp`) | Jira issues, Confluence pages, Compass components, Bitbucket, and cross-product search | Atlassian OAuth 2.1 or API token | `official` `jira` `confluence` |
| Calendly | [MCP Server documentation](https://developer.calendly.com/calendly-mcp-server) (`https://mcp.calendly.com`, HTTPS) | List and manage event types, inspect availability, list available times, and update availability schedules | Calendly account and OAuth 2.1 Authorization Code with PKCE and Dynamic Client Registration; scheduling read/write scopes | `official` `scheduling` `appointments` |
| ClickUp | [MCP server documentation](https://developer.clickup.com/docs/connect-an-ai-assistant-to-clickups-mcp-server) (`https://mcp.clickup.com/mcp`, HTTP) | Workspace tasks, Lists, Folders, Docs, comments, time tracking, and Chat workflows | ClickUp OAuth 2.1 with PKCE | `official` `project-management` `tasks` |
| HubSpot | [MCP server documentation](https://developers.hubspot.com/ai-tools/mcp) (`https://mcp.hubspot.com`) | CRM objects, engagements, contacts, companies, deals, tickets, and commerce records | HubSpot OAuth 2.0 (user-level MCP app) | `official` `crm` `sales` |
| Linear | [MCP server guide](https://linear.app/docs/mcp) (`https://mcp.linear.app/mcp`) | Issues, projects, comments, and planning workflows | Linear OAuth or API key | `official` `project-management` `issues` |
| monday.com | [MCP integration guide](https://developer.monday.com/api-reference/docs/integrate-with-monday-mcp) (`https://mcp.monday.com/mcp`) | Boards, items, documents, and workflows through 60+ read/write tools | monday.com OAuth 2.0 or personal API token | `official` `project-management` `workflows` |
| Salesforce Hosted MCP | [Hosted MCP server documentation](https://developer.salesforce.com/docs/platform/hosted-mcp-servers/guide/hosted-mcp-servers-overview.html) (`https://api.salesforce.com/platform/mcp/v1/platform/sobject-all`) | Salesforce object CRUD, queries, search, Data 360, Tableau, and configurable Apex/Flow tools across hosted servers | Salesforce OAuth 2.0 with PKCE; an org admin must enable the server; URLs vary by org and server | `official` `crm` `enterprise` |
| ServiceNow | [MCP server documentation](https://www.servicenow.com/docs/r/intelligent-experiences/create-mcp-server.html) (`https://<instance>.service-now.com/sncapps/mcp-server/mcp/<server-name>`) | Configurable tools for IT, HR, and business workflows exposed from a ServiceNow instance | ServiceNow subscription/entitlement, admin-created server, and OAuth inbound integration | `official` `itsm` `automation` |

### Media and Content

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| ElevenLabs | [Official source repository](https://github.com/elevenlabs/elevenlabs-mcp) (`uvx elevenlabs-mcp`, stdio) | Text-to-speech, speech-to-text, voice cloning and design, sound effects, music, and voice agents | ElevenLabs API key | `official` `audio` `speech` |
| Vimeo | [MCP server documentation](https://developer.vimeo.com/api/mcp-server) (Claude `https://mcp.vimeo.com/mcp`; ChatGPT `https://mcp.vimeo.com/sse`, remote HTTPS) | Search videos, inspect metadata, transcripts, chapters, comments, captions, and analytics; manage showcases and video metadata/privacy | Vimeo account and video library; plan-dependent capabilities; beta | `official` `video` `media` |

### Search and Research

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| AWS Knowledge | [MCP server documentation](https://awslabs.github.io/mcp/servers/aws-knowledge-mcp-server) (`https://knowledge-mcp.global.api.aws`, Streamable HTTP) | Search and read current AWS documentation, API references, troubleshooting and architecture guidance, What's New, CDK/CloudFormation, and agent skills | None; public service is rate-limited and does not require an AWS account | `official` `aws` `documentation` |
| Brave Search | [Official source repository](https://github.com/brave/brave-search-mcp-server) (`npx -y @brave/brave-search-mcp-server`, stdio) | Web, local business, place, image, video, and news search, plus LLM context and AI summarization | Brave Search API key and plan; optional HTTP mode is unauthenticated by default and should be protected | `official` `web-search` `local-search` |
| Context7 | [MCP client setup](https://context7.com/docs/resources/all-clients) (`https://mcp.context7.com/mcp`, Streamable HTTP) | Resolve libraries and retrieve current, version-specific documentation and code examples | Optional API key; OAuth or Bearer auth enables higher limits and private repositories | `official` `documentation` `libraries` |
| Exa | [Web Search MCP documentation](https://exa.ai/docs/reference/exa-mcp) (`https://mcp.exa.ai/mcp`, Streamable HTTP) | Web and code search, full-page retrieval, advanced search, and multi-step research with Exa Agent | Exa OAuth or API key; free usage is available on the hosted service | `official` `web-search` `research` |
| Firecrawl | [MCP server documentation](https://docs.firecrawl.dev/mcp) (`https://mcp.firecrawl.dev/{FIRECRAWL_API_KEY}/sse`, SSE) | Web search, scraping, crawling, content extraction, deep research, and batch scraping | Firecrawl API key | `official` `web-scraping` `extraction` |
| Google Developer Knowledge | [MCP connection guide](https://developers.google.com/knowledge/mcp) (`https://developerknowledge.googleapis.com/mcp`, Streamable HTTP) | Search and retrieve official Google developer documentation, code samples, release notes, and grounded answers | Google Cloud OAuth or API key; project and service enablement required | `official` `documentation` `search` |
| Microsoft Learn | [MCP server reference](https://learn.microsoft.com/en-us/training/support/mcp-developer-reference) (`https://learn.microsoft.com/api/mcp`, Streamable HTTP) | Search Microsoft Learn documentation, fetch pages, and find code samples | None for the public endpoint | `official` `documentation` `search` |
| Perplexity | [MCP server documentation](https://docs.perplexity.ai/docs/getting-started/integrations/mcp-server) (`https://api.perplexity.ai/mcp`, Streamable HTTP) | Real-time web search, conversational answers, and advanced reasoning | Perplexity API key | `official` `web-search` `reasoning` |
| Tavily | [MCP server documentation](https://docs.tavily.com/documentation/mcp) (`https://mcp.tavily.com/mcp`, Streamable HTTP) | Real-time web search, web-page extraction, and site mapping | Tavily OAuth or API key | `official` `web-search` `extraction` |

### Browser and Automation

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Browserbase | [MCP server setup](https://docs.browserbase.com/integrations/mcp/setup) (`https://mcp.browserbase.com/mcp`, Streamable HTTP) | Browser navigation, interaction, screenshots, extraction, and Stagehand agent workflows | Browserbase API key; custom models may require a separate model key | `official` `browser` `automation` |
| Zapier | [MCP client guide](https://help.zapier.com/hc/en-us/articles/36265392843917-Use-Zapier-MCP-with-your-client) (`https://mcp.zapier.com/api/v1/connect`) | Connect AI clients to actions across Zapier's 9,000+ app ecosystem | Zapier connection token (Bearer) | `official` `automation` `workflows` |

### AI and LLM

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Braintrust | [MCP documentation](https://www.braintrust.dev/docs/integrations/developer-tools/mcp) (US `https://api.braintrust.dev/mcp`; EU `https://api-eu.braintrust.dev/mcp`, Streamable HTTP) | Search documentation, inspect experiments, logs, datasets, and prompts, query data with SQL, summarize experiments, and generate permalinks | Braintrust OAuth 2.0 or API key; data-plane endpoint varies by region | `official` `evaluation` `observability` |
| Hugging Face | [MCP server documentation](https://huggingface.co/docs/hub/en/agents-mcp) (`https://huggingface.co/mcp`, remote HTTP) | Search models, datasets, Spaces, papers, and documentation; run Jobs and sandboxes; use community Spaces tools | Hugging Face account; client-specific setup is generated in MCP settings | `official` `models` `datasets` |
| LangSmith | [MCP server documentation](https://docs.langchain.com/langsmith/langsmith-mcp-server) (`https://langsmith-mcp-server.onrender.com/mcp`, HTTP) | Conversation history, prompts, traces and runs, projects, datasets, experiments, evaluations, and billing usage | LangSmith API key in the `LANGSMITH-API-KEY` header; workspace and endpoint headers are optional | `official` `evaluation` `tracing` |
| Replicate | [MCP server documentation](https://replicate.com/docs/reference/mcp) (`https://mcp.replicate.com/sse`, SSE) | Discover and compare models, inspect model metadata, and create and manage predictions through Replicate's API | Replicate OAuth or API token | `official` `models` `inference` |

### Data and Databases

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Airtable | [MCP server guide](https://support.airtable.com/v1/docs/using-the-airtable-mcp-server) (`https://mcp.airtable.com/mcp`) | Bases, tables, schemas, records, comments, and workspace data | Airtable OAuth or PAT | `official` `databases` `no-code` |
| BigQuery | [Use the BigQuery MCP server](https://docs.cloud.google.com/bigquery/docs/use-bigquery-mcp) (`https://bigquery.googleapis.com/mcp`, Streamable HTTP) | List datasets and tables, inspect schemas, and run read-only or full SQL queries | Google Cloud OAuth; project IAM roles and BigQuery API enablement required | `official` `sql` `data-warehouse` |
| MongoDB | [MCP server documentation](https://www.mongodb.com/docs/mcp-server/overview/) ([official source repository](https://github.com/mongodb-js/mongodb-mcp-server); `npx -y mongodb-mcp-server@latest --readOnly`, stdio) | Query and inspect databases and schemas; manage Atlas resources; use Performance Advisor and MongoDB knowledge search | MongoDB connection string or Atlas service-account credentials; read-only mode is recommended | `official` `mongodb` `database` |
| Neon | [MCP server overview](https://neon.com/docs/ai/neon-mcp-server) (`https://mcp.neon.tech/mcp`) | Projects, branches, databases, SQL, schema changes, and branch-based migrations | Neon OAuth or API key for remote agents | `official` `postgres` `database` |
| Pinecone | [MCP server documentation](https://docs.pinecone.io/guides/operations/mcp-server) (`npx -y @pinecone-database/mcp`, stdio) | Search Pinecone documentation, manage indexes, upsert records, query indexes, and rerank results | Pinecone API key | `official` `vector-search` `database` |
| PostHog | [MCP documentation](https://posthog.com/docs/model-context-protocol) (`https://mcp.posthog.com/mcp`, Streamable HTTP) | Product analytics, HogQL, feature flags, experiments, session replay, error tracking, CDP, and support workflows | PostHog account authentication; US/EU data-region routing | `official` `analytics` `feature-flags` |
| Snowflake | [Snowflake-managed MCP server documentation](https://docs.snowflake.com/en/user-guide/snowflake-cortex/cortex-agents-mcp) (`https://<account_url>/api/v2/databases/<database>/schemas/<schema>/mcp-servers/<name>`) | Cortex Analyst, Cortex Search, Cortex Agents, custom tools, and governed SQL execution | Snowflake OAuth by default or External OAuth; account/database/schema/server setup required | `official` `data-warehouse` `analytics` |
| Supabase | [MCP server documentation](https://supabase.com/docs/guides/ai-tools/mcp) (`https://mcp.supabase.com/mcp`) | Project-scoped database, docs, debugging, development, functions, branching, and storage tools | Supabase OAuth or PAT | `official` `database` `backend` |

### Developer Tools

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| GitHub | [Remote server setup](https://github.com/github/github-mcp-server/blob/main/docs/remote-server.md) (`https://api.githubcopilot.com/mcp/`) | Repositories, issues, pull requests, code search, and Actions | GitHub OAuth or PAT | `official` `repositories` `issues` |
| GitLab | [MCP server documentation](https://docs.gitlab.com/user/model_context_protocol/mcp_server/) (`https://gitlab.com/api/v4/mcp`, HTTP) | Project information, issues, merge requests, and GitLab API operations | GitLab OAuth 2.0 Dynamic Client Registration; group or instance enablement required; Beta | `official` `repositories` `issues` |
| LaunchDarkly | [Hosted MCP server documentation](https://launchdarkly.com/docs/home/getting-started/mcp-hosted) (`https://mcp.launchdarkly.com/mcp/launchdarkly`) | Feature flags, AgentControl configs, observability logs, traces, errors, dashboards, and metrics | LaunchDarkly OAuth; hosted server excludes federal and EU environments | `official` `feature-flags` `observability` |
| Postman | [Remote MCP server setup](https://learning.postman.com/latest-v-12/docs/reference/postman-api/postman-mcp-server/postman-mcp-remote-server) (`https://mcp.postman.com/mcp`) | Workspaces, collections, specifications, mocks, monitors, environments, and API workflows | Postman OAuth on the US remote server; API key required for the EU remote server | `official` `api-testing` `workspaces` |
| Twilio | [MCP server documentation](https://www.twilio.com/docs/ai/mcp) (`https://mcp.twilio.com/docs`) | Search Twilio, SendGrid, and Segment API documentation and retrieve endpoint schemas across 1,800+ endpoints | None; public API specifications only | `official` `api-docs` `schemas` |

### Cloud and Infrastructure

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Cloudflare API | [Managed MCP server documentation](https://developers.cloudflare.com/agents/model-context-protocol/cloudflare/servers-for-cloudflare/) (`https://mcp.cloudflare.com/mcp`) | DNS, Workers, R2, Zero Trust, and other Cloudflare API operations through search and execute tools | Cloudflare OAuth or scoped API token | `official` `cloud` `workers` |
| Vercel | [MCP server documentation](https://vercel.com/docs/agent-resources/vercel-mcp) (`https://mcp.vercel.com`) | Documentation search, project and deployment management, and deployment-log analysis | Vercel OAuth | `official` `hosting` `deployments` |

### Monitoring and Security

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Datadog | [MCP server documentation](https://docs.datadoghq.com/mcp_server/) (`https://mcp.datadoghq.com/v1/mcp`, US1) | APM, logs, metrics, monitors, dashboards, security signals, and observability workflows | Datadog OAuth 2.0, PAT/SAT, or API/application keys | `official` `observability` `monitoring` |
| Grafana Cloud | [Cloud MCP server documentation](https://grafana.com/docs/grafana-cloud/ai-tools/mcp-servers/cloud-mcp/) (`https://mcp.grafana.com/mcp`) | Metrics, logs, dashboards, alerts, incidents, investigations, and other Grafana Cloud observability data | Grafana OAuth 2.1; Grafana Cloud role/permission and Assistant access required | `official` `observability` `metrics` |
| New Relic | [MCP setup](https://docs.newrelic.com/docs/agentic-ai/mcp/setup/) (US `https://mcp.newrelic.com/mcp/`; EU `https://mcp.eu.newrelic.com/mcp/`, HTTP) | Observability discovery, NRQL/data access, alerting, incident response, performance analytics, and advanced analysis | New Relic OAuth or API key; region-specific endpoint; Preview | `official` `observability` `monitoring` |
| Sentry | [MCP server documentation](https://mcp.sentry.dev/) (`https://mcp.sentry.dev/mcp`) | Error issues, events, traces, performance, projects, releases, and debugging workflows | Sentry OAuth | `official` `error-tracking` `observability` |

### Science and Computation

| Provider / server | Connection details | Capabilities | Auth | Tags |
| --- | --- | --- | --- | --- |
| Wolfram Cloud MCP | [Remote MCP documentation](https://www.wolfram.com/artificial-intelligence/mcp/cloud/wolfram-mcp-cloud/) (`https://agenttools.wolfram.com/mcp`, Streamable HTTP) | Wolfram\|Alpha knowledge, Wolfram Language evaluation, and contextual computation and documentation tools | No API key required for Wolfram MCP Service; client/account access may apply | `official` `computation` `knowledge` |

## Legend

**Auth** identifies the credentials or account needed to use a server; `none`
should be used only when the server truly requires no authentication.

The `official` tag means the provider publishes or maintains the linked
server. Other tags should describe the server's primary capability, not serve
as a second category system.

Links point to the provider's official endpoint, connection documentation, or
source repository. Each provider retains ownership of its software,
trademarks, data, and licenses.

## Contributing

Contributions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) for the
acceptance criteria and pull request format.

## Maintainer

0mcp.io creates and maintains Awesome Public MCP Servers. This curated list is
dedicated to the public domain under [CC0 1.0 Universal](LICENSE). Linked MCP
servers and documentation remain subject to their respective owners' licenses
and terms.
