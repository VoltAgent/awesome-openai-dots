# Engineering & Product Use Cases

[← Back to main list](../README.md#use-cases)

These are **proposed** workflows, not prebuilt dots. Availability and actions depend on the connected apps, account, workspace, and product surface. Review every draft before it changes shared project data.

## Weekly project pulse

- **Apps:** [GitHub](https://chatgpt.com/plugins/plugin_connector_1p_1a69035c238881919c4190932b2df699), [Slack](https://chatgpt.com/plugins/slack), and optionally [Notion](https://chatgpt.com/plugins/notion).
- **Trigger:** A weekly schedule or an explicit request.
- **Workflow:** Review recent pull requests, issue updates, and linked project notes; group progress, blockers, and decisions; cite the source links.
- **Output:** A concise weekly status draft organized by project, progress, and blockers.
- **Human review:** Verify the summary and approve it before sharing or changing issues.

## Release readiness review

- **Apps:** [GitHub](https://chatgpt.com/plugins/plugin_connector_1p_1a69035c238881919c4190932b2df699), [Vercel](https://chatgpt.com/plugins/vercel), and the team's project tracker.
- **Trigger:** A release candidate or a requested pre-release check.
- **Workflow:** Compare the release checklist with open changes, required checks, preview deployment, and documentation; list gaps with evidence.
- **Output:** A go/no-go checklist with unresolved items and links to their sources.
- **Human review:** A person decides whether to merge, deploy to production, or change production data.

## Design-to-deployment handoff

- **Apps:** [Figma](https://chatgpt.com/plugins/figma), [GitHub](https://chatgpt.com/plugins/plugin_connector_1p_1a69035c238881919c4190932b2df699), and [Vercel](https://chatgpt.com/plugins/vercel).
- **Trigger:** A design marked ready for implementation.
- **Workflow:** Summarize the approved design, identify the related issue or pull request, and collect the preview link and implementation notes.
- **Output:** A handoff checklist linking the design, code change, and preview.
- **Human review:** A designer or engineer confirms the design version and checks the preview before release.

## Customer feedback to product backlog

- **Apps:** [Slack](https://chatgpt.com/plugins/slack), [Notion](https://chatgpt.com/plugins/notion), and [Linear](https://chatgpt.com/plugins/linear).
- **Trigger:** A feedback review or a recurring weekly triage.
- **Workflow:** Group feedback by theme, link each theme to its source, compare it with existing product notes, and draft candidate issues.
- **Output:** A deduplicated feedback summary and proposed Linear issues.
- **Human review:** Confirm priority, remove personal or confidential details, and approve each issue before creation.

## Database change impact review

- **Apps:** [GitHub](https://chatgpt.com/plugins/plugin_connector_1p_1a69035c238881919c4190932b2df699), [Supabase](https://chatgpt.com/plugins/plugin_asdk_app_69d3e5ee6a708191baa733f7b8931995), and [Notion](https://chatgpt.com/plugins/notion).
- **Trigger:** A database migration pull request or a requested review.
- **Workflow:** Compare the proposed migration with the documented schema and related code; flag destructive operations, missing rollback notes, or unclear assumptions.
- **Output:** A migration review checklist with file and documentation links.
- **Human review:** A database owner validates the findings and approves any migration or production action.

## Project deadline check

- **Apps:** [Linear](https://chatgpt.com/plugins/linear), [Google Calendar](https://chatgpt.com/plugins/google-calendar), and [Todoist](https://chatgpt.com/plugins/plugin_asdk_app_6943b73823548191a9f9216c6790c453).
- **Trigger:** A weekly planning session or an upcoming milestone.
- **Workflow:** Compare assigned work and due dates with calendar availability; flag conflicts and missing owners without changing schedules automatically.
- **Output:** A short list of deadline risks and proposed next actions.
- **Human review:** The project owner confirms priorities and approves calendar or task changes.
