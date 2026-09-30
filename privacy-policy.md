---
title: Privacy Policy
---

# Habits Softly Privacy Policy

**Effective 30 September 2026**

Habits Softly is a habit-tracking app for iPhone and Android made by an independent developer. This policy explains what the app stores, why, who else touches it, and how you delete it. It is written to be read, not skimmed past: if something here is unclear, email **habitssoftly@gmail.com** and we will answer plainly.

## The short version

- You need an account (email and password, or Sign in with Apple / Google). Your habits sync to it so they are the same on every device you sign in on.
- We store what you put in: your habits, check-ins, challenges, settings, and optionally a name and a profile photo.
- We do not sell data, show ads, use advertising or analytics SDKs, or track you across other apps or websites.
- Once a week and once a day, the app can have an AI service (Anthropic's Claude) reword a summary of your habit numbers. It receives habit names and counts only, never your email, name, photo or account ID.
- You can delete your account and every piece of data from inside the app (Manage tab → Account → Delete account). It is immediate and permanent.

## What we collect and why

| Data | Why | Where it lives |
|---|---|---|
| Email address, password (stored only as a hash by Supabase; we never see it) | Signing in; password reset | Supabase Auth |
| Apple or Google identity token (when you use those buttons); the email and first name they share | Signing in without a password; a greeting | Supabase Auth; the name in your profile |
| Display name (optional) | Greetings in the app and in a reminder | Your profile |
| Profile photo (optional) | Shown in the app | Supabase Storage, at a random unguessable address; a copy on your phone |
| Habits (name, icon, colour, target, reminder time, days), daily check-in counts, challenges, streak freezes, settings (sound, reminders, check-in times) | The app itself | Your phone (local database) and Supabase, synced |
| Push token, platform (iOS/Android), time zone, when the app was last opened, how many "come back" nudges were sent | Delivering reminders across your devices; sending at most three gentle nudges at 6 pm your time if the app has not been opened for three days, then stopping | Supabase |
| A cached copy of AI-worded summaries, keyed by week or day | So the same summary is not generated twice | Supabase, deleted with your account |

We do not collect your precise or approximate location, contacts, health data, device identifiers for advertising, browsing history, or anything from other apps. The app does not use your microphone or camera except when you choose to take a profile photo, and then only to take that photo.

## Where data is stored

Your account and synced data are hosted by **Supabase** (Supabase, Inc.) in its Canada (Central) region on Amazon Web Services. Data is encrypted in transit (TLS) and at rest. Each account can read and write only its own rows; this is enforced by the database itself (row-level security), not just by the app.

A copy of your habits and settings is kept on your phone so the app opens instantly and works offline. It lives in the app's private storage and is removed when you sign out or delete the app.

## Who else processes data

We use a small number of service providers, each for one job. None of them may use your data for their own purposes.

| Provider | What they receive | Job |
|---|---|---|
| Supabase, Inc. | Everything in the table above | Hosting: accounts, database, file storage, server functions |
| Anthropic, PBC | Habit names, counts, streak lengths, percentages, challenge titles, weekday names | Rewording the weekly reflection and the daily nudge. Anthropic's API does not train on this data. No account identifiers are sent. |
| Expo (650 Industries, Inc.), Apple Push Notification service, Google Firebase Cloud Messaging | Your push token and the text of each push notification (which may include your first name) | Delivering push notifications |
| Brevo (Sendinblue SAS) | Your email address and the reset link | Sending password-reset emails |
| Apple (Sign in with Apple), Google (Google Sign-In) | Handled under their own policies when you choose those buttons | Identity |

We do not use advertising networks, analytics or crash-reporting SDKs, or social-media SDKs.

## Reminders and notifications

Habit reminders are scheduled on your phone. If you have more than one device, a silent push tells the others to update so a habit checked off on one stops reminding you on another. If you turn reminders off in the app, no push notification of any kind is sent, including the "your habits are waiting" nudge. You can also turn notifications off in your phone's settings at any time.

## How long we keep data

For as long as your account exists. Deleting your account deletes everything listed above, immediately, including push tokens, cached AI summaries and your profile photo. Our hosting provider may hold short-lived backups for disaster recovery; they expire automatically and are never used for anything else.

## Deleting your account

In the app: **Manage tab → Account → Delete account**. This is available on every platform, needs no email or waiting period, and cannot be undone.

If you can no longer sign in, email **habitssoftly@gmail.com** from the address on the account and we will delete it within 7 days and confirm.

## Your rights

Wherever you live, you can ask us to show you, correct, export or delete the personal data we hold about you, and you can withdraw consent to optional processing (such as reminders or the profile photo) at any time from inside the app. Email **habitssoftly@gmail.com**. If you are in the EU/EEA or UK you also have the right to complain to your data-protection authority; if you are in California, we do not sell or share personal information as those terms are defined in the CCPA/CPRA.

## Children

Habits Softly is not directed to children under 13 (or the minimum age for consent in your country) and we do not knowingly collect data from them. If you believe a child has created an account, email us and we will delete it.

## Security

Passwords are hashed by Supabase Auth and never visible to us. All traffic uses TLS. Server secrets (such as the AI service key) live only on the server, never in the app. Sign-in and password-reset endpoints are rate-limited. We reviewed the app against a security checklist before release and will continue to.

## Changes

If this policy changes in a way that matters, the effective date above changes, the update's release notes say so, and the new version is published at the same address before it takes effect. Older versions are available on request.

## Contact

**habitssoftly@gmail.com**
