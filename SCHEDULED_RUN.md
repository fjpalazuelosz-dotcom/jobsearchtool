# Automation instructions for ONE search-and-publish run

Adapt placeholders after the new Site exists. The new account's automation tool stores the schedule separately from this prompt. Do not put schedule text alone in the Site source and call it configured.

```text
Run one job-search update for {{CANDIDATE_NAME}} and publish the result to the NEW Site {{NEW_SITE_PROJECT_ID}} at {{NEW_SITE_URL}}. Read the Site owner's currently saved location and target-role preferences first; use the configured defaults only if none are saved. Use the authoritative CV attached to this Project and the constraints in NEW_USER_CONFIG. Do not rely on another account's Site or private data.

Determine today's date in {{TIME_ZONE}}. Calculate and state the exact inclusive original-posting window {{WINDOW_RULE}}. Search eligible hybrid/onsite and remote scopes independently; confirm that remote roles explicitly allow the candidate's location. Search by responsibilities and titles. Look at LinkedIn Jobs first, Indeed second, Google Jobs third, then the priority employers' official career/ATS pages and other relevant employers. Note access blocks instead of implying a source was searched. Exclude configured employers and hard disqualifiers.

Open employer or direct ATS evidence for original posting date, location/work model, and current open application. Relative age, crawl time or repost date is not an original date. Page failure alone is not closure. Reverify every Probable fit record, including ones marked Interested or Applied, and check existing verified roles for continued availability. Keep strong unresolved leads visible with exact gaps. Retain closed/ineligible records with evidence. Deduplicate and promote in place, preserving stable IDs, URL aliases, user choices and prior verification history.

Add up to {{MAX_NEW_RESULTS}} distinct strongest newly verified roles, never padding. Rate fit 1–10 against demonstrated CV facts; keep combined pros/cons under 100 words. Label employer-stated salary POSTED with currency and period. Otherwise use a credible {{SALARY_MARKET}} estimate labeled ASSUMPTION with source, or unavailable. Prepare truthful role-focused PDF CV drafts for fit >= {{FIT_SCORE_THRESHOLD}}, preserving substantial original history. Do not submit applications.

Update both Site records and the latest-run report, including search time, exact local window, checked sources, unresolved evidence, additions, changes and no-new-results outcome. Open the NEW Site source using authorized Sites access, build, push the exact source, save a version, deploy and inspect its status. Report failure if publication fails. Notify the owner only according to {{NOTIFICATION_RULE}}; otherwise update quietly. Never claim the live Site changed until the deployment succeeds.
```

## Schedule construction

For an exact daily schedule, use the new user's IANA time zone and hours from `NEW_USER_CONFIG`. For example, Pala's *reference* schedule was:

```ical
BEGIN:VEVENT
DTSTART;TZID=America/Mexico_City:20260929T120000
RRULE:FREQ=DAILY;BYHOUR=8,10,12,14,16,18,20,22;BYMINUTE=0;BYSECOND=0
END:VEVENT
```

The DTSTART above was only an example valid on its date. Calculate a fresh next occurrence for the new account and replace both the timezone and hours as required. Use exact scheduling for explicit clock times. Make only one task for this Site; check existing tasks before creating another. Verify the first real execution and publication.
