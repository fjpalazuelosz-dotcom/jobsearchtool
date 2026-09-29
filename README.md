# Reusable Job Watch Site kit

A copy-and-paste specification for building a **new person's** job-search Site in a **different ChatGPT account**. It reproduces the Pala Job Watch workflow and visual structure without assuming access to the original account, source repository, CV, jobs, or private storage.

**Reference design:** [Pala Job Watch](https://pala-job-watch.noemimtzo.chatgpt.site/) as observed September 29, 2026 (version 58). This repository is documentation, not a source-code export or a credential bundle. It is safe to adapt for a new person only after replacing all placeholders and supplying that person's CV.

## Files

| File | Purpose | Where to use it |
| --- | --- | --- |
| [`docs/NEW_USER_CONFIG.md`](docs/NEW_USER_CONFIG.md) | Fill-in profile, criteria, schedule, privacy and publishing choices | Copy into the new ChatGPT Project as a message or attached file |
| [`prompts/PROJECT_INSTRUCTIONS.md`](prompts/PROJECT_INSTRUCTIONS.md) | Boundaries and recurring operating rules | Paste into the new Project's Instructions field |
| [`prompts/CREATE_SITE.md`](prompts/CREATE_SITE.md) | One-time build and deployment request | Paste as the first message in the new Project |
| [`prompts/SCHEDULED_RUN.md`](prompts/SCHEDULED_RUN.md) | Single-run instructions for the automation | Use when creating or reviewing the scheduled task |
| [`docs/ACCEPTANCE.md`](docs/ACCEPTANCE.md) | Verification checklist and limits | Use before saying the copy is complete |

## Quick start in another account

1. Copy this documentation to your GitHub repository. Keep the repository private if you add a real CV, job decisions, contact information, or generated PDFs. The files in this kit contain placeholders rather than personal data.
2. Make a copy of `docs/NEW_USER_CONFIG.md`. Fill **every required field** for the new person. Choose the eligible geography, role families, exclusions, employers, and schedule for that person; do not assume Jalisco or Pala's criteria apply.
3. In the **new person's ChatGPT account**, create a new Project. Attach the person's authoritative CV to that Project or paste its complete text there. Paste the completed configuration as a Project file or message. The CV is necessary for truthful fit scores and complete tailored PDFs.
4. Paste `prompts/PROJECT_INSTRUCTIONS.md` into the Project Instructions field. Replace the `{{CONFIG_FIELD}}` placeholders with values from the completed configuration if the Project does not reliably read the file.
5. Paste `prompts/CREATE_SITE.md` as a new message in the Project. This authorizes creation of a **new** Site and scheduled task in that account. The agent must make a new Sites project, new storage, and a new automation. It must not reuse the original Pala project ID or try to access private data from its URL.
6. Review the new deployed Site against `docs/ACCEPTANCE.md`. The agent should report the new URL, project ID, successful deployment, schedule configuration, and what still needs a real scheduled run to verify.
7. After the first scheduled run, check its actual timestamp, exact local date window, research evidence, saved Site version, and live update. An enabled task is not proof of end-to-end publication.

## What copy and paste can reproduce

The prompts specify the five-view dashboard, visual language, job model, decisions, PDF behavior, search rules, publishing workflow, and schedule. They can direct an enabled Sites-capable account to **build a functional equivalent from scratch**.

Text cannot carry the original HTML/CSS/Worker source, exact pixels, seed job records, the candidate's full CV, PDF files, private decisions, authenticated account identity, storage, API keys, or automation state. A byte-for-byte clone requires an authorized source export and those assets. The public Pala URL is only a visual reference and does not provide private source or data. Do not claim an exact clone from this documentation alone.

## Reference behavior to preserve

The dashboard has **Job watch**, **Probable fit**, **Interested**, **Not interested**, and **Right now**. Job watch has one collapsible **Search Criteria** panel with editable criteria and a compact type scale 25% below normal body text. Cards are individually expandable. There is no Run search button, Check me maybe? tab, or Save for later button. Interested/Not interested actions move the card to its category **without switching the current view**. Applied is manual; no application is submitted by the Site.

The source reference schedule was daily at 08:00, 10:00, 12:00, 14:00, 16:00, 18:00, 20:00, and 22:00 `America/Mexico_City`. This is an **example**. Set the new user's schedule and timezone in the configuration. The run window is the fourteen complete local calendar days before the search date unless the new user's configuration intentionally changes it.

## Maintaining this repository

Update the configuration template and three prompts together when behavior changes. Keep a date and version note for material revisions. Never commit secrets, private storage dumps, CVs without consent, or an unredacted source export to a public repository. GitHub holds these instructions; a GitHub commit alone does not publish a ChatGPT Site or create a ChatGPT Automation.

