# Awesome OpenAI Dots

A community-curated collection of workflows, rules, plugins, integrations, and practical guides for OpenAI dots in ChatGPT.

> **Unofficial community project.** Not affiliated with or endorsed by OpenAI.

Dots are always-on agents in ChatGPT that can work toward ongoing goals, use a cloud computer, and work with apps you choose to connect. This list focuses on practical ways to use and extend dots, with clear notes about permissions, approvals, and availability.

## Contents

- [Official OpenAI resources](#official-openai-resources)
- [Workflow ideas](#workflow-ideas)
- [What belongs here](#what-belongs-here)
- [Important boundaries](#important-boundaries)
- [Contributing](CONTRIBUTING.md)

## Official OpenAI resources

### Dots: product and user guides

- [Introducing dots](https://openai.com/index/introducing-dots/) — Product overview, capabilities, examples, permissions, safeguards, and rollout.
- [Meet dots](https://learn.chatgpt.com/docs/dots) — Official ChatGPT Learn landing page for the dots documentation.
- [Getting started with your dot](https://learn.chatgpt.com/docs/dots/getting-started) — Create a dot and start assigning it work.
- [Message your dot](https://learn.chatgpt.com/docs/dots/channels) — Reach a dot across supported messaging channels.
- [Tasks and memory](https://learn.chatgpt.com/docs/dots/tasks-and-memory) — Ongoing tasks, schedules, and memory.
- [Connect computers and apps to your dot](https://learn.chatgpt.com/docs/dots/computers-and-apps) — Connected apps and computer access.
- [Control your dot](https://learn.chatgpt.com/docs/dots/controls) — Custom Rules, approvals, and activity controls.
- [Getting started with your dot — Help Center](https://help.openai.com/en/articles/20001530-getting-started-with-your-dot) — Setup, plan and regional availability, tasks, memory, and controls.
- [Dots privacy, security, and safety FAQs](https://help.openai.com/en/articles/20001529-dots-privacy-security-and-safety-faqs) — Data access, connected apps, Custom Rules, Auto-review, and safeguards.

### Plugins and integrations

- [Plugins in ChatGPT](https://help.openai.com/en/articles/20001256-plugins-in-chatgpt) — Plugins can bundle reusable skills, connected apps, and other capabilities; includes creation, sharing, and permissions.
- [Connect and manage app accounts](https://help.openai.com/en/articles/20001494-connecting-and-managing-app-accounts-in-chatgpt) — Account setup, authorization, and disconnecting apps.
- [Import and sync plugin marketplaces from GitHub](https://help.openai.com/en/articles/20001504-importing-and-syncing-plugin-marketplaces-from-github) — Workspace admins can import marketplaces from public or private GitHub repos. The guide documents `.agents/plugins/marketplace.json` and the daily sync behavior.

### Admin and safety references

- [Manage dots in ChatGPT workspaces](https://help.openai.com/en/articles/20001554-manage-dots-in-chatgpt-workspaces) — Enterprise workspace controls for dots, computers, connected apps, and messaging.
- [GPT-6 Astra System Card](https://deploymentsafety.openai.com/gpt-6-astra/evaluating-auto-review) — Model and agent safety evaluations, including dot-specific safeguards and red-team findings.

## Workflow ideas

These are starting points based on scenarios in OpenAI’s announcement. They are ideas to adapt and test, not prebuilt or OpenAI-approved dots.

- **Engineering feedback loop:** Monitor recurring customer feedback, propose a small fix, test it, and return a pull request for review.
- **Research watch:** Recheck selected sources on a schedule, compare new evidence with the research question, and surface changes for review.
- **Launch coordination:** Track scope changes and prepare updated launch notes, assets, or project documents as drafts.
- **Content production:** Turn a new interview transcript into proposed clips, show notes, and social drafts for approval.
- **Sales proposal upkeep:** Compare new requirements with product documentation, update a draft proposal, and flag unresolved commitments.

Community submissions should include the connected apps required, setup steps, expected output, and which actions are read-only, require approval, or change external data.

## What belongs here

- Tested dot workflows and reusable task recipes.
- Custom Rules examples with a clear explanation of their limits.
- Plugins and connected-app integrations that dots can use, including setup and permission requirements.
- Guides for recurring tasks, messaging, cloud/local computer access, memory, and review.
- Safety checklists, troubleshooting notes, and evaluations based on reproducible scenarios.
- Specialist-dot patterns for organization workflows, where access to the relevant feature is available.

## Important boundaries

- **A dot is a ChatGPT product, not a downloadable agent package.** Do not claim a workflow is an installable dot unless OpenAI provides that capability and the entry has been verified.
- **A plugin is a real extension path.** OpenAI documents plugins containing reusable skills and connected apps, and documents importing a plugin marketplace from GitHub. A dot can use supported connections within the permissions granted to its owner.
- **Private marketplace imports are workspace-admin functionality.** Importing a marketplace does not connect users’ app accounts or grant access. Review all entries before importing; later syncs can bring in new plugins automatically.
- **Custom Rules do not override built-in safeguards.** Clearly disclose actions that need approval and any external side effects.
- **Availability changes.** Dots and individual capabilities are rolling out and can depend on plan, region, surface, and workspace settings. Check the linked official docs before relying on a workflow.

## Source review

Official links and feature notes last checked **2026-09-30**. Please open an issue or pull request when an official URL changes or a capability moves out of rollout.
