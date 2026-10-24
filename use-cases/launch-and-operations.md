# Launch & Operations Use Cases

[← Back to main list](../README.md#use-cases)

These are **proposed** workflows, not prebuilt dots. Confirm app availability and permissions, and require approval before external communication or publishing.

## Launch content workspace

- **Apps:** Product docs in [Google Drive](https://chatgpt.com/plugins/plugin_connector_1p_ab21a553bfbc81919ea8fd1858e3ffa7) or [Notion](https://chatgpt.com/plugins/notion), plus [Adobe](https://chatgpt.com/plugins/adobe-photoshop) or [Canva](https://chatgpt.com/plugins/canva).
- **Trigger:** A launch date or a request from the launch owner.
- **Workflow:** Collect approved product facts, draft a launch brief and channel-specific copy, and prepare visual assets for review.
- **Output:** A launch checklist, copy drafts, and links to draft assets.
- **Human review:** Check claims, assets, and copy before anything is published or sent externally.

## Support trend report

- **Apps:** Permitted [Slack](https://chatgpt.com/plugins/slack) or [Gmail](https://chatgpt.com/plugins/plugin_connector_1p_95d39881713c8191931482a62d6edff9) conversations and product docs in [Drive](https://chatgpt.com/plugins/plugin_connector_1p_ab21a553bfbc81919ea8fd1858e3ffa7) or [Notion](https://chatgpt.com/plugins/notion).
- **Trigger:** A weekly schedule.
- **Workflow:** Group recurring issues, compare them with product documentation, remove identifying details, and include links to relevant source records where policy allows.
- **Output:** An anonymized report of common issues, emerging changes, and documentation gaps.
- **Human review:** Check privacy and accuracy; keep draft replies unsent until approved.

## Sales account preparation

- **Apps:** [Apollo.io](https://chatgpt.com/plugins/apollo), [HubSpot](https://chatgpt.com/plugins/hubspot), and [Gmail](https://chatgpt.com/plugins/plugin_connector_1p_95d39881713c8191931482a62d6edff9).
- **Trigger:** A scheduled account review or an upcoming sales conversation.
- **Workflow:** Combine permitted CRM notes with approved company research, highlight recent context and unanswered questions, and draft a tailored agenda or email.
- **Output:** An account brief and unsent communication draft.
- **Human review:** Confirm recipient, claims, and tone before updating CRM records or sending messages.

## E-commerce campaign preparation

- **Apps:** [Shopify](https://chatgpt.com/plugins/shopify), [Adobe](https://chatgpt.com/plugins/adobe-photoshop) or [Canva](https://chatgpt.com/plugins/canva), and optionally [Google Drive](https://chatgpt.com/plugins/plugin_connector_1p_ab21a553bfbc81919ea8fd1858e3ffa7).
- **Trigger:** A new product, promotion, or seasonal campaign.
- **Workflow:** Collect approved product details, prepare draft listing copy and creative briefs, and compare required assets with the campaign checklist.
- **Output:** Product-page copy drafts, asset checklist, and campaign readiness notes.
- **Human review:** Verify product facts, pricing, and creative rights; a person approves edits and publication in the store.

## Inbox-to-action triage

- **Apps:** [Outlook Email](https://chatgpt.com/plugins/outlook-email), [Outlook Calendar](https://chatgpt.com/plugins/outlook-calendar), and [Todoist](https://chatgpt.com/plugins/plugin_asdk_app_6943b73823548191a9f9216c6790c453).
- **Trigger:** A daily review or an explicit request.
- **Workflow:** Group messages by urgency and topic, identify likely tasks or meeting requests, and draft a proposed plan without replying or scheduling automatically.
- **Output:** A prioritized inbox summary and proposed tasks or calendar slots.
- **Human review:** Confirm task details, invitations, and all outgoing responses before they are created or sent.

## Weekly training recap

- **Apps:** [COROS](https://chatgpt.com/plugins/coros) or [Fitness AI Connector](https://chatgpt.com/plugins/fitness-ai-connector).
- **Trigger:** A weekly schedule or a request to review recent activity.
- **Workflow:** Summarize recorded training and activity trends from the connected account; avoid diagnosing symptoms or prescribing treatment.
- **Output:** A personal activity recap with trends and questions to discuss with a qualified professional if needed.
- **Human review:** Check the data and sharing permissions; do not use the recap for urgent or clinical decisions.

## Weekly domain health watch

- **Label:** Community workflow using a third-party custom MCP app; **Proposed** (not run end to end in a dot). Disclosure: submitted by Datawright Labs, which makes the Apify tools it uses. Not an OpenAI or Apify listing.
- **Apps:** A custom MCP app pointing at [Apify's MCP server](https://docs.apify.com/integrations/chatgpt) with the Datawright Labs DNS, SSL, WHOIS/RDAP and broken-link tools ([source and tool list](https://github.com/datawright-labs/datawright-agent-tools)). Not in the ChatGPT plugin directory.
- **Requirements:** ChatGPT with Developer mode (custom MCP apps) and dots access; a free Apify account. Runs are billed per result on that Apify account (about $0.001 per domain checked).
- **Setup:** Settings > Apps & Connectors (Plugins) > Create. MCP Server URL `https://mcp.apify.com?tools=datawright-labs/email-domain-dns-checker,datawright-labs/ssl-certificate-checker,datawright-labs/whois-rdap-domain-lookup,datawright-labs/broken-link-checker`, Authentication OAuth (sign in to Apify, no client ID). Tools are fixed when the app is created; re-create it to change them.
- **Trigger:** A weekly schedule, e.g. "Every Monday, check SPF, DMARC, DKIM, SSL expiry, domain expiry and broken links for mydomain.com and tell me only if something is wrong."
- **Workflow:** Run the read-only checks on the listed domains and site, fetch the result rows with the server's `get-dataset-items` tool, and compare with last week.
- **Output:** A short alert listing only problems: failing email-auth records, certificates or domain registrations expiring soon, and broken links with the page they appear on.
- **Human review:** None needed for the checks themselves (they only read public DNS, TLS, RDAP and web pages); a person decides on any DNS, certificate or site fixes.
- **Verified:** 2026-10-24. Setup steps from Apify's ChatGPT integration docs; the MCP URL was tested to list these tools over Streamable HTTP outside ChatGPT. Not yet tested inside ChatGPT or a dot.
