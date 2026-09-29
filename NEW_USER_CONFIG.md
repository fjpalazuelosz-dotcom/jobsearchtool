# New user configuration — fill before creating the Site

Copy this template for each new person. Replace every `{{...}}` value. Attach the person's complete authoritative CV separately in their ChatGPT Project; do not rely on a short summary when creating tailored CVs. Do not put a private CV or contact details in a public GitHub repository without the person's consent.

## Identity and access

- Site title: `{{SITE_TITLE}}` (example: “Alex's Job Watch”)
- Candidate name to display: `{{CANDIDATE_NAME}}`
- Site owner's ChatGPT account: `{{OWNER_ACCOUNT}}` (identify through authenticated Sites access; do not hardcode someone else's email)
- Initial audience: `{{OWNER_PRIVATE_OR_PUBLIC}}` (recommended: owner-private until the candidate reviews the content)
- Authoritative CV: `{{ATTACHED_CV_FILENAME_OR_COMPLETE_TEXT_IN_PROJECT}}`
- CV language(s): `{{CV_LANGUAGES}}`
- Contact details permitted on public pages/PDFs: `{{CONTACT_SHARING_RULES}}`
- Existing job records to import: `{{NONE_OR_AUTHORIZED_DATA_FILE}}`
- Existing decisions to import: `{{NONE_OR_AUTHORIZED_EXPORT}}` (default: none)

## Search profile

- Local time zone (IANA): `{{TIME_ZONE}}` (example: `America/Mexico_City`)
- Eligible hybrid/onsite geography: `{{HYBRID_LOCATION}}`
- Eligible remote geography: `{{REMOTE_COUNTRY_OR_REGION}}`; the listing must explicitly allow the candidate's location
- Work models to include: `{{WORK_MODELS}}`
- Target titles and equivalent responsibilities: `{{TARGET_ROLES}}`
- Priority employers: `{{PRIORITY_EMPLOYERS}}`
- Excluded employers: `{{EXCLUDED_EMPLOYERS}}`
- Required languages, legal work eligibility, travel or other hard constraints: `{{HARD_CONSTRAINTS}}`
- Maximum distinct newly verified results per run: `{{MAX_NEW_RESULTS}}` (Pala reference: 10)
- Original posting-date window: `{{WINDOW_RULE}}` (Pala reference: 14 **complete** local calendar days before the run, today minus 14 through yesterday)
- Salary currency and geography for estimates: `{{SALARY_MARKET}}`
- Notification rule: `{{MATERIAL_CHANGES_ONLY_OR_OTHER}}`

## Schedule

- Schedule enabled? `{{YES_OR_NO}}`
- Exact daily times in local time: `{{LOCAL_TIMES}}` (Pala example: `08:00,10:00,12:00,14:00,16:00,18:00,20:00,22:00`)
- No-run hours: `{{NO_RUN_WINDOW}}` (Pala example: `00:00–07:59`)
- First eligible start date/time: `{{NEXT_LOCAL_OCCURRENCE}}` (calculate when creating the task)
- Recurrence days: `{{EVERY_DAY_OR_WEEKDAYS_ETC}}`

## Content and approval choices

- Use the Pala visual structure (navy/white/teal, five views, compact expandable cards): `{{YES_OR_SPECIFY_CHANGES}}`
- PDF CV draft threshold: `{{FIT_SCORE_THRESHOLD}}` (Pala reference: 7/10)
- Allow the user to mark Applied manually: `{{YES_OR_NO}}`
- Allow automatic application submission: **NO**
- Keep a role with uncertain original date/work model/application in Probable fit: **YES**
- Publish after each completed scheduled run: `{{YES_OR_NO}}`

## Preflight confirmation

- [ ] Candidate supplied and authorized use of the complete CV.
- [ ] Search geography and remote eligibility are explicit.
- [ ] Target roles, exclusions and hard constraints are complete.
- [ ] Site audience and CV contact-sharing rules are clear.
- [ ] Schedule times and time zone are filled; there is no duplicate automation.
- [ ] The new account has Sites and Automations access, or the agent will report the specific blocker.
