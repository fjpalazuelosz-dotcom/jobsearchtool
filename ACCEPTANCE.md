# Acceptance checklist for a new user's Site

Record the evidence, not just a yes/no assertion. A new account cannot inherit Pala's test results.

## Inputs and ownership

- [ ] New candidate's full CV is available in their Project and consented for this use.
- [ ] The Site title, owner identity, audience, search geography, roles, exclusions, salary market, notification rule, time zone and schedule match the completed configuration.
- [ ] The Site has a NEW project ID, storage and automation. No reference-account ID, email, private decision, credential or stale candidate fact appears in its source or UI.
- [ ] Public pages and PDFs expose only permitted contact information.

## UI and decisions

- [ ] Five views in the specified order; no Run search, Check me maybe? or Save for later control.
- [ ] One merged Search Criteria panel; its preference editor works and its displayed schedule matches the actual task. Check desktop and mobile widths and keyboard operation.
- [ ] Cards show each required field and expand independently. Verified and probable classifications match displayed evidence.
- [ ] From Job watch and Probable fit, Interested and Not interested move the card to the intended tab while the current tab stays selected.
- [ ] Applied is manual; no site action submits an application.
- [ ] Browser decisions survive reload. Owner-authenticated choices and personal preferences restore in another browser/session. Simulate a save failure and confirm pending/retry behavior.
- [ ] Any migrated legacy maybe records remain visible without restoring removed controls.

## CV, salary and research

- [ ] PDF downloads for fit scores at or above threshold open correctly and retain significant history, education and credentials from the authoritative CV. No invented qualification.
- [ ] Salary POSTED is supported by the ad with currency and period; ASSUMPTION has a local market source; unavailable is explicit.
- [ ] First run states its exact local time and inclusive posting window. If run on September 29, 2026 with the Pala 14-day rule, the window is September 15–28, 2026; calculate new windows from the actual date/time.
- [ ] LinkedIn, Indeed, Google Jobs, and official employer/ATS checks are recorded honestly. Remote eligibility is explicit. Probable leads retain precise unresolved fields. No duplicate or lost user decision after promotion.

## Publication and automation

- [ ] Build/test commands pass and the exact source commit is pushed to the new Site repository.
- [ ] A saved version is deployed successfully. Record new project ID, version, deployment ID, URL and publish time.
- [ ] Exactly one enabled automation has the configured IANA timezone and local recurrence, including its no-run hours.
- [ ] A real scheduled run executed, reached its sources, updated records and latest-run report, saved a new version, deployed successfully, and changed the live Site. If unverified, label this step **pending**.
- [ ] A search or publication failure is visible as a failure; it is not represented as “no new jobs.”

## Evidence log template

| Check | Result | Evidence / URL / timestamp | Owner |
| --- | --- | --- | --- |
| First Site deployment | Pending | | |
| Signed-in persistence | Pending | | |
| PDF/CV factual review | Pending | | |
| First scheduled execution | Pending | | |
| Scheduled live publication | Pending | | |
