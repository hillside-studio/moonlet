---
title: Moonlet Privacy Policy
permalink: /privacy/
lang: en
---

# Moonlet Privacy Policy

**Effective date:** 8 November 2026
**Developer:** Hillside Studio ("we", "us")
**Contact:** hillside.studio.dev@gmail.com

Moonlet helps you put your phone down at night. It does not lock your phone. When you are past
your bedtime goal and still scrolling, it shows a short pause and lets you choose what to do next.

This policy explains what Moonlet knows about you, where that information stays, and the two
optional features that send anything off your phone.

## The short version

- **No account.** You never sign up or log in.
- **Your data stays on your phone.** Your bedtime, the apps you pick, your nightly history and
  anything you write are stored only on your device.
- **No ads and no analytics.** Moonlet has no advertising and no analytics or tracking tools.
- **Two optional features send limited data, and both are off until you turn them on:**
  1. **Crash reports**, sent to Sentry, our crash-reporting provider.
  2. **Smart messages**, short summaries sent through our server to our AI provider, the company
     whose AI model writes the messages: OpenAI or Anthropic, depending on how our server is
     configured.
- **Your notes never leave your phone.** What you type in "Write it down" is never sent to us,
  Sentry or our AI provider.
- **You can delete everything** from the Me tab, or by uninstalling the app.

## 1. What Moonlet stores on your phone

Moonlet stores the following in the app's private storage on your device (an SQLite database and
Android app preferences). Other apps cannot read it. We cannot read it either.

| What | Why |
|---|---|
| Your bedtime goal, and the optional sentence you wrote about why it matters to you | To know when to check in, and to remind you of your own reason |
| The apps you chose to watch | So Moonlet only checks in when you are in those apps |
| Your settings (nudge strength, morning check-in times, pause for tonight, crash-report and smart-message switches) | To work the way you set it up |
| Your nightly history: when each check-in happened, which watched app was open, the reason you picked (for example "Just unwinding"), what you chose, roughly when you put the phone down, and your morning answer ("Worth it", "It was OK", "Regret it") | To show your nights in Review and write your weekly summary |
| Things you chose to "talk about tomorrow", and notes you write with "Write it down" | To bring them up in the morning review, if you want |
| Usage sessions for the apps you chose (app, start and end time, length) | To work out how long you have been scrolling tonight |

**Backups.** Your nights, notes and "Write it down" text are never included in your phone's
cloud backup. Depending on your phone's backup settings, Android may back up Moonlet's settings
(your bedtime goal, the apps you chose, nudge strength) to your own Google account. That backup is
handled by Google under your account, not by us, and we cannot access it. If you move to a new
phone with a direct phone-to-phone transfer, your records can come along.

## 2. Permissions Moonlet asks for

Moonlet asks for each permission only when you reach the step that needs it, and explains why
first. You can turn any of them off later in Android settings; Moonlet will keep working as far as
it can and tell you what is missing.

- **Usage access** (Android setting "Usage access"). Lets Moonlet see which app is in the
  foreground and for how long. It does **not** let Moonlet see what you watch, read or type inside
  those apps. Moonlet only looks at this during your evening watch window (from 30 minutes before
  your bedtime goal until early morning), only cares about the apps you chose, and keeps the
  results on your phone.
- **Display over other apps** (Android setting "Display over other apps"). Lets Moonlet show its
  night check-in on top of the app you are using. Moonlet shows it only when a check-in is due,
  and you can always close it.
- **Notifications.** Used for the bedtime reminder, the morning check-in and the weekly summary,
  and for the ongoing notification Android requires while Moonlet is keeping watch at night.
- **Run at startup.** After your phone restarts, Moonlet reschedules its evening check so it keeps
  working without you opening the app.
- **Foreground service.** While Moonlet is keeping watch at night it runs as a foreground service
  with an ongoing notification ("Guarding your bedtime"), so Android does not stop it halfway
  through the evening. It stops on its own outside the watch window or when you turn monitoring
  off.
- **Internet.** Used only for the two optional features below.

Moonlet also looks at the list of apps installed on your phone that can be opened from the home
screen, so you can choose which ones to watch. That list is used on your phone only.

## 3. Optional: crash reports (off by default)

If you turn on **Send crash reports** in the Me tab, Moonlet sends a report to
[Sentry](https://sentry.io) (Functional Software, Inc.), our crash-reporting provider, when the app
crashes or hits a serious error. We use these reports only to find and fix bugs.

A crash report contains:

- technical details of the error: the error type and stack trace, meaning which part of the app's
  code failed. The error message is removed before sending, because it could contain text;
- information about the app and phone: app version, Android version, phone manufacturer and model,
  language, time zone, and technical state such as memory and storage;
- a short trail of recent system events before the crash (for example the app going to the
  background, or the network changing). Taps and typing are not recorded;
- a random identifier created by the crash-reporting tool for this installation, so we can tell
  whether one install or many are affected. It is not linked to your name, email or Google account.

A crash report does **not** contain your notes, your "talk about tomorrow" text or your reason
sentence. Moonlet sends a report only when something goes wrong; it does not report each time
you open the app.

Sentry, like any internet service, receives your IP address when the report is uploaded.
We have configured Sentry not to store IP addresses.

Sentry keeps crash reports for up to 90 days and then deletes them. You can turn
crash reports off at any time in the Me tab; nothing more is sent after that.

## 4. Optional: smart messages (off by default)

If you turn on **smart messages**, Moonlet uses an AI model to write some of its messages in a more
personal way: the reply after your morning check-in, the summary in your weekly review, and the
wording of the night check-in. With smart messages off, Moonlet uses built-in messages instead and
works fully.

### What is sent

Moonlet sends only the short summaries listed below. It never sends the names of the apps you use,
anything you saw in other apps, your contacts, your "Write it down" notes, or your "talk about
tomorrow" text.

**After a morning check-in** (at most once a morning, after a night with a check-in):

- the app language;
- your bedtime goal and the time you put the phone down last night;
- how many check-ins there were last night, and the reasons you picked (for example "Can't stop");
- your morning answer ("Worth it", "It was OK" or "Regret it");
- whether you saved something to talk about (yes/no only, not what it was);
- a summary of your recent nights: how many nights, how many you regretted, how many were worth it,
  and how far, on average, your phone-down time was from your goal.

**For the weekly summary** (at most once a week): the app language and, for each of up to 7 nights,
the day of the week, your bedtime goal, your phone-down time, the number of check-ins, the reasons
you picked and your morning answer.

**For the night check-in wording** (at most once an evening, prepared in advance): the app language,
your bedtime goal, the sentence you wrote about why your bedtime matters to you (at most 140
characters), and the same recent-nights summary as above.

Every request also carries:

- a **random device identifier** created by Moonlet when you install it. It is not linked to your
  name, email, Google account or advertising ID. We use it only to limit how many requests one
  install can make per day.
- a **Google Play Integrity token**, which lets our server check that the request comes from a
  genuine copy of Moonlet installed from Google Play. Google processes integrity checks under its
  own terms; see the Play Integrity link at the end of this policy.

### Who receives it

1. **Our server** (a small proxy that we operate, hosted on Cloudflare Workers). It checks the
   request, accepts only the fields listed above, and forwards them to the AI model. It adds
   nothing about you. **It does not store the content of your requests or the replies.** It
   records only a short technical line per request (which feature, whether it worked, how long it
   took), with no content and no device identifier. Cloudflare, like any internet service, sees
   your IP address when the request arrives; our server does not record it.
2. **Our AI provider**, which provides the AI model that writes the message. This is **OpenAI**
   (model: GPT) **or Anthropic** (Anthropic, PBC; model: Claude), depending on how our server is
   configured. Only one of them receives a given request. The provider processes the request to
   produce the reply.
   - **OpenAI:** API data is not used to train OpenAI's models. We ask OpenAI not to store the
     request or reply, but OpenAI keeps abuse-monitoring logs of API requests for up to 30 days.
   - **Anthropic:** API inputs and outputs are not used to train Anthropic's models, and are
     deleted within 30 days. Anthropic may keep them longer, up to 2 years, if they are flagged as
     violating its usage policy, or where the law requires.

Data is sent over encrypted connections (HTTPS).

You can turn smart messages off at any time in the Me tab. From then on nothing more is sent.

## 5. Your safety

If something you write suggests you may be in crisis, Moonlet shows a page with ways to get help:
a link to [findahelpline.com](https://findahelpline.com) and your local emergency number. This check
runs entirely on your phone using simple word lists. It is not done by AI, and nothing is sent
anywhere. Moonlet is not a medical or emergency service.

## 6. Children

Moonlet is meant for adults (18 and over). It is not directed at children, and we do not
knowingly collect personal information from children. Moonlet does not ask for your age or name.
If you believe a child has turned on crash reports or smart messages and want related data removed,
contact us at hillside.studio.dev@gmail.com.

## 7. Sharing and selling

We do not sell your data. We do not share it with anyone for advertising. The only outside
companies that receive any data are the providers named above (Sentry, if you turn on crash
reports; Cloudflare and our AI provider, OpenAI or Anthropic, if you turn on smart messages), and
only so they can provide that feature for us. We may disclose information if required by law, but
we hold very little: we do not store your smart-message requests, and crash reports are the only
data we keep.

## 8. How long data is kept, and deleting it

- **On your phone:** until you delete it. Use **Delete all data** in the Me tab to erase your
  history, notes and settings from the phone. Uninstalling Moonlet also removes all of its data
  from the phone (separately, Android may keep a copy of your settings in your own Google backup, as described in
  section 1).
- **Smart messages:** not stored by our server. Our AI provider may keep them for a limited time, as
  described in section 4.
- **Crash reports:** kept by Sentry for up to 90 days and then deleted. Because crash reports
  are not linked to your identity, we may not be able to find yours; if you want us to try, email
  hillside.studio.dev@gmail.com and we will delete any we can identify.

## 9. Security

Your data lives in Moonlet's private app storage, which Android keeps separate from other apps.
Anything Moonlet sends uses encrypted connections (HTTPS). Our server keeps its access keys secret,
accepts requests only from genuine copies of the app, and limits how many requests each install can
make.

## 10. Your rights

Depending on where you live, you may have rights to access, correct or delete your personal data,
or to object to how it is used. Because almost everything stays on your phone, you can see, change
and delete it yourself in the app. For anything else, contact hillside.studio.dev@gmail.com.

## 11. Changes to this policy

If we change this policy, we will update the effective date above and, for important changes, tell
you in the app before the change applies to you.

## 12. Contact

Hillside Studio
hillside.studio.dev@gmail.com
