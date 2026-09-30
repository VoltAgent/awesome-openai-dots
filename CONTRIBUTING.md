# Contributing

Thanks for helping make this a useful, accurate resource for OpenAI dots.

## What to submit

Submit a use case, Custom Rules example, plugin/app listing, connected-app guide, safety resource, or troubleshooting note that is relevant to dots. Prefer primary documentation and hands-on reports over vague claims. Add entries to the relevant file under `categories/` or `use-cases/`, rather than growing the root README into a giant catalog.

## Entry requirements

Include:

- A concise name and description.
- What problem it solves and who it is for.
- The required plan, region, ChatGPT surface, workspace role, and connected apps, if known.
- Setup steps and a representative task or example.
- What the dot can read or change, and which steps need approval.
- A date and the version or rollout state you verified.
- A public source link. Do not include credentials, private workspace details, or real user data.

For a use case, include the required plugins/apps (with verified directory links where available), the workflow trigger or schedule, the expected output, and the human review points. Mark it **Proposed** if it has not been run end to end; use **Tested** only with a short, reproducible test note.

Clearly label whether an entry is an OpenAI-published resource, a community workflow, or a third-party plugin. Do not imply OpenAI endorsement.

## Where entries go

- Add ChatGPT plugin/app directory listings to the matching category file under `categories/`.
- Add OpenAI GitHub plugin source folders to the full inventory in `categories/openai-github-plugins.md`. Link to the source folder, not to a guessed ChatGPT listing.
- Add workflows to the matching file under `use-cases/`. Link back to the relevant plugin and app categories.
- Add a new category or use-case page only when the existing sections do not fit; add its link to the root README table of contents.

## Plugin and marketplace submissions

For plugin/app listings, include the verified ChatGPT directory detail link and, when available, a separate source repository or package link. Do not guess detail-page URLs or claim two similarly named entries are the same without checking.

For plugin packages, document required apps, permissions, authentication, supported surfaces, and any external side effects. A GitHub marketplace can be imported by an eligible workspace admin; importing processes valid entries and future syncs may add new plugins. Keep marketplace changes small and review them before merging.

## Pull requests

- Keep each pull request focused.
- Verify every link and capability claim.
- Explain how you tested the workflow without exposing private information.
- Update the source review date when changing official-resource notes.
