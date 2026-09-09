# Anchor Privacy Policy

**Effective date:** September 5, 2026 (first version July 11, 2026)
**App:** Anchor (listed on the App Store as “Anchor: Routine OS”)
**Operator:** Sahad Chowdhury (sole developer)
**Contact:** sec.5707@gmail.com

Anchor is a routine planner. This policy explains exactly what data the app handles, where it goes, and what never leaves your phone. It is written to be read, not skimmed past.

## The short version

- Your **routine data** (anchors, items, day levels, check-ins) syncs to our server so it survives reinstalls and moves between your devices. It is yours, tied to your account, and deleted when you delete your account.
- Your **Apple Health data and calendar details never leave your phone.**
- **No ads. No tracking. No analytics SDKs. No selling or sharing data for marketing. Ever.**

## What we collect (leaves your device)

| Data | What exactly | Why |
|---|---|---|
| Account email | The email you sign up with, or the one Apple shares when you use Sign in with Apple (which may be a private relay address) | Sign-in, account recovery |
| Routine content | Your anchors, routine items, day levels, expectations, and check-in logs (what you completed, skipped, or excused, and logged amounts) | Sync and backup — this *is* the app’s content |
| Calendar link (identifier only) | If you link an anchor to a calendar event, an opaque event identifier is stored with that anchor | So the link survives across your devices. Event titles, times, attendees, and any other calendar details are **not** synced |
| Account identifiers | The random account id your rows are filed under, and a second random id used only to exclude your data from any future engine training | Sign-in, row-level security, and the training opt-out |
| Install identifier | A random id created once per app install (not your device's advertising or vendor id) and attached to each plan you accept | So a plan change can be attributed to the install that made it, which is how sync conflicts are diagnosed |

This data is stored in our database (Supabase, hosted in the United States) and is isolated to your account by row-level security.

## What stays on your device (never transmitted)

- **Apple Health data.** If you connect Health, Anchor reads sleep, heart-rate variability, resting heart rate, and — only if you enable it — cycle data, entirely on-device, to suggest an easier day or anchor your morning. None of it is uploaded, and Anchor never writes to Health.
- **Calendar details.** Event contents are read on-device to place your anchors.
- **Notification schedules and app preferences.**

Our commitments on health data: it is never used for advertising or marketing, never mined, never sold, never written to iCloud, and never sent to our server. If a future feature ever needs a health-derived signal to sync, we will update this policy and ask for your explicit in-app consent **first** — it will never be silent.

## What we don’t do

- No advertising, and no advertising identifiers.
- No tracking across apps or websites (our privacy manifest declares zero tracking domains).
- No third-party analytics or crash-reporting SDKs.
- No selling, renting, or sharing of your data for anyone’s marketing.

## Service providers

Two providers process data on our behalf, strictly to run the app: **Supabase** (database, authentication, and functions hosting) and **Apple** (Sign in with Apple). Neither is permitted to use your data for anything else.

## Retention and deletion

Your data is kept while your account exists. **Settings → Delete account** permanently deletes your account, your profile, and every routine row tied to it — anchors, items, day levels, expectations, day logs, check-ins, plans, outcomes — immediately, and wipes the app’s local data. If you signed in with Apple, we also revoke the app’s Sign in with Apple grant. You can export everything first (Settings → Export my data) as JSON.

One record survives deletion: the two random account identifiers above, with the time of deletion and **no routine content**. It exists so that a phone that was offline during the deletion can never re-upload deleted data, and so the deletion itself is auditable. It contains nothing that identifies you outside our database, and it is never used for any other purpose.

## Your rights

Access and portability are built in (the export button). Deletion is built in (the delete button). For anything else — including questions, complaints, or rights under GDPR, UK GDPR, CCPA, or similar laws — email sec.5707@gmail.com and we will respond within 30 days. You may also lodge a complaint with your local supervisory authority.

## Children

Anchor is not directed at children under 13 (or the equivalent minimum age in your region), and we do not knowingly collect their data.

## Changes

If this policy changes, the new version will be posted at this address with a new effective date. Material changes to how health-adjacent data is handled will additionally be surfaced in the app before they apply to you.
