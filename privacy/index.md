---
layout: default
title: "Privacy Policy – Eisenhower AI"
lang: en
---

[Türkçe](/eisenhower-ai-legal/privacy/tr/)

# Eisenhower AI – Privacy Policy

Effective date: 8 October 2026

This policy explains what personal data the Eisenhower AI iPhone and iPad app
("the app") and its optional online services handle, why, where it goes, how long
it is kept, and what rights you have. A Turkish version, which also serves as the
information notice (*aydınlatma metni*) under Article 10 of the Turkish Personal
Data Protection Law No. 6698 ("KVKK"), is available at the same address. If you
use the app in Türkiye, the Turkish version is the one that counts.

## 1. Who is responsible

The data controller is:

- Anil Goral
- Postal address: given on request by email
- Email: goralanil@gmail.com

"We", "us" and "our" in this policy mean the controller.

EU representative: none appointed.

KVKK data controller registry (VERBIS): not registered. The controller is a natural person whose main activity is not processing personal data, and who falls under the Personal Data Protection Board's exemption from registration for controllers with fewer than 50 employees and an annual balance sheet below the Board's threshold.

## 2. The short version

- **Your tasks stay on your device.** The app has no cloud sync. We cannot see
  your task list.
- **No analytics, no advertising, no tracking.** The app contains no analytics,
  crash-reporting or advertising software, and we do not track you across apps or
  websites.
- **AI Capture is optional.** If you use it, the text you type into AI Capture is
  sent to our AI service to be sorted, and the result comes back to your device.
  Our service does not save that text or the AI's answer.
- **An account is only needed for the paid AI service.** It is created with Sign
  in with Apple. We ask Apple for an email address, which can be Apple's Hide My
  Email address, and never for your name. You can delete the account in the app.
- **Payments are handled by Apple.** We never see your card or bank details.

## 3. Data that stays on your device

Everything you put into the app's task list is stored only on your device:

- **Tasks.** Each task is saved as a Markdown file in the app's own folder
  ("Eisenhower AI Next" in the app's Documents folder). A task file holds its
  title, notes, quadrant, status, dates and reminder times, recurrence, tags,
  timestamps and, for tasks created with AI Capture, the text the task came from
  and the AI's suggestion and reasoning.
- **A backup copy.** The app keeps a second copy of your task list, and your app
  settings, in a small database in the same Documents folder, so that a damaged
  file cannot lose your list.
- **Deleted tasks.** Deleting a task moves its file to a hidden trash folder
  inside the app's folder. It stays there until you delete the app.
- **Sign-in and security keys.** If you sign in, the app keeps your account
  identifier and a sign-in refresh token in the iOS Keychain. If you use AI
  Capture, it keeps the identifier of its App Attest key there too (see
  section 4). These Keychain items are set to stay on this device only.
- **Reminders.** Reminders are local notifications scheduled on your device. A
  reminder shows the task's title, which can appear on your lock screen
  depending on your iOS notification settings. We do not use push notifications
  and do not receive any notification token.

The app's Documents folder is visible in the iOS Files app, so you can open,
copy or back up your tasks yourself. It is also included in your normal iCloud
or computer backups of the device, which Apple or your computer handles under
your own settings. We have no access to any of it.

To remove all of this from your device, delete the app. Deleting your account
(section 6) does not delete the tasks on your device.

## 4. AI Capture

AI Capture turns a block of text into suggested tasks. It is optional: the app
also offers "No AI", which splits your text into tasks on your device, leaves
them unsorted for you to place, and sends nothing anywhere.
Before AI Capture first sends anything, the app shows you what will be sent and
where, and asks you to continue. You can withdraw that choice in Settings → AI at
any time; withdrawing stops future requests but cannot undo requests already
processed.

**What is sent.** When you submit an AI Capture, the app sends:

- the text you entered (up to 8,000 characters);
- your device's language and region setting (for example `tr-TR`) and time
  zone, so that words like "tomorrow" are understood correctly;
- a random request number created for that one request;
- App Attest data that proves the request comes from a genuine copy of the app
  (see below);
- when accounts are switched on, a sign-in token that identifies your account,
  so that your subscription and allowance can be checked.

**Where it goes.** The request travels over an encrypted connection through
Cloudflare, which carries traffic to our service, to a gateway and an AI model
that run on a computer we operate ourselves. No other AI company receives your
text. The suggestions come back to your device, and nothing is added to your
task list until you review and confirm it.

**What our service keeps.** The gateway uses your text only in memory to answer
that request. It does not write the text, or the AI's answer, to disk or to its
logs, and it is not used to train or improve any AI model. If operational
logging is switched on, a log line contains only the random request number, the
service name, how many items were sent, how long the request took and whether it
succeeded.

**Country.** Cloudflare tells our gateway which country a request comes from,
based on its network address, so that we can apply country restrictions. We do
not store it.

**App Attest.** To keep the service from being abused, the app uses Apple's App
Attest. The first time you use AI Capture, the app asks Apple to create a key
that belongs to this installation of the app and sends us Apple's confirmation.
Our gateway keeps a record of that key on our computer: its identifier, its
public key, a counter that stops old requests from being replayed, the
environment, and the dates it was created, last updated or revoked. This record
contains no task text and is not linked to your account. We keep it for
12 months after its last use; it is then deleted automatically.

**Please do not put sensitive information into AI Capture** – for example
health details, or other people's personal data – unless you need to. The text
is processed only to give you suggestions, but it does leave your device.

## 5. Account and subscription

You only need an account to use the paid AI Capture service.

**Sign in with Apple.** The app signs you in with Apple and asks Apple for your
email address, never your name. Apple lets you share your real address or a Hide
My Email address that forwards to it. Apple gives the app a sign-in token, which
the app exchanges with our account provider, Supabase, for a session. From then
on your account is identified by a random user identifier.

We need the email address for two reasons: Supabase cannot create an account
without one, and it is how your iPhone sign-in and a desktop sign-in belong to
the same account. If you also use the Eisenhower AI desktop app, which signs in
with an email address and a password, and the confirmed address there matches
the one Apple gives us, both are the same account and share one subscription.
We do not use it for marketing.

**What Supabase stores for us** (in its Frankfurt, Germany data centre):

- your user identifier and Apple's identifier for you in our app, which links
  your Apple sign-in to your account;
- the email address Apple gives us, which may be a Hide My Email address;
- the session records Supabase needs to keep you signed in, which can include
  the network address and app identifier of the sign-in;
- your plan (free or paid), when your current subscription ends, and the time of
  the last subscription update we received;
- a usage counter: how many AI Capture requests you have made in the current
  30-day period, and when that period started;
- if you also sign in to the Eisenhower AI desktop app: for each computer, an
  identifier, its public key, and when it was added, last used and signed out.

Supabase does not store your tasks or your AI Capture text.

**Computers on your account.** The account screen lists the computers signed in
to your account, with the date each was added and last used, and lets you sign
them all out at once. A signed-out computer has to sign in again before it can
use AI Capture.

**Signing out.** When you sign out, the app tells Supabase to end your session,
so the stored sign-in token stops working on the server too, and removes your
account identifier and sign-in token from the device. It also switches the
purchase service on this device back to an anonymous identity. If the device is
offline, it still signs out locally, and the old session expires on its own.

**Purchases.** Subscriptions are sold through the App Store. Apple handles
payment, and we never receive your payment details. The app uses RevenueCat to
manage subscriptions: it passes RevenueCat your account identifier, and
RevenueCat receives your App Store purchase and subscription records (such as
the product, purchase and renewal dates and status) from Apple and the app.
RevenueCat tells our system when your subscription starts, renews, is refunded
or ends, and we record only the plan and end date listed above.

## 6. How long we keep data

| Data | How long |
|---|---|
| Tasks, backup copy, trash and settings on your device | Until you delete them or the app. We have no copy. |
| AI Capture text and AI answers | Not kept by us after the request is answered. |
| App Attest record on our computer | 12 months after its last use, then deleted automatically. |
| Account at Supabase: user identifier, Apple identifier, email address, sessions | Until you delete your account. |
| Plan, subscription end date and usage counter | Until you delete your account. The counter is reset at the start of each 30-day period and at each purchase or renewal. |
| Computer keys | Until you delete your account. A signed-out computer's key is kept, marked as signed out, so it can never be used again. |
| Customer record at RevenueCat | Until you ask us to delete it (see below). |
| Purchase records at Apple | As set by Apple for its own legal and accounting duties. |
| Emails you send us | As long as needed to deal with your request and any follow-up. |

**Deleting your account.** You can delete your account in the app: Settings → AI
→ Account and subscription → Delete account. Before anything is deleted, the app
reminds you that deleting the account does not cancel an App Store subscription,
and Apple asks you to confirm with Sign in with Apple. Deleting then:

1. signs out every computer connected to the account;
2. deletes your plan, subscription end date and usage counter, and every
   computer key;
3. revokes the app's Sign in with Apple authorisation, so the app no longer
   appears under Sign in with Apple in your Apple Account. If this step cannot be
   completed, the app tells you how to remove it yourself in iOS Settings;
4. deletes your account at Supabase: your user identifier, Apple identifier,
   email address and sessions;
5. signs you out on the device.

What it does not delete:

- **Your App Store subscription.** Cancel it yourself at
  apps.apple.com/account/subscriptions or in your Apple ID settings, or Apple
  keeps charging you.
- **The customer record at RevenueCat**, which holds your old account identifier
  and purchase history. It is not deleted automatically. Email goralanil@gmail.com
  and we will delete it by hand.
- **Apple's own purchase records.**
- **The tasks on your device.** Delete the app to remove them.

If RevenueCat reports a late subscription change for a deleted account, our
system may recreate a bare record holding only the old random identifier and
the plan. It contains no email address and nobody can sign in to it; we delete
it on request.

If you cannot use the app, you can also email us to ask for deletion.

## 7. Why we use data, and our legal grounds

| Purpose | Data | Legal ground (GDPR / KVKK) |
|---|---|---|
| Providing AI Capture | Capture text, language/region, time zone, request number | Performing our contract with you (GDPR Art. 6(1)(b); KVKK Art. 5(2)(c)) |
| Your account and subscription, including the fair-use allowance and linking your iPhone and desktop sign-ins | User identifier, Apple identifier, email address, plan, end date, usage counter, computer keys | Performing our contract with you (GDPR Art. 6(1)(b); KVKK Art. 5(2)(c)) |
| Protecting the service from abuse: App Attest, rate limits, country restrictions | App Attest record, request timing, country of the request | Our legitimate interest in a secure, fairly shared service (GDPR Art. 6(1)(f); KVKK Art. 5(2)(f)) |
| Answering your requests and meeting legal duties | Your messages and the data needed to act on them | Legal obligation (GDPR Art. 6(1)(c); KVKK Art. 5(2)(ç)) and our contract with you |
| Establishing or defending legal claims | Only the data relevant to the claim | Legitimate interest (GDPR Art. 6(1)(f)); establishing, exercising or protecting a right (KVKK Art. 5(2)(e)) |

You do not have to use AI Capture or create an account; the rest of the app
works without them. If you do not provide the data AI Capture needs, we cannot
provide AI Capture.

AI Capture suggests where tasks belong. It does not make decisions about you
that have legal or similarly significant effects, and you review every
suggestion before it is saved.

## 8. Who receives data

We do not sell personal data or share it for advertising. We use these service
providers, each only for the job described:

| Provider | What it does | Where |
|---|---|---|
| Cloudflare, Inc. | Carries AI Capture traffic to our computer over an encrypted tunnel and protects it from attacks. It necessarily handles the request in transit, including your network address, and keeps network and security logs under its own policies. | United States and Cloudflare's global network |
| Supabase, Inc. | Hosts our account database and sign-in service. | Frankfurt, Germany (EU) |
| RevenueCat, Inc. | Manages App Store subscriptions. | United States |
| Apple | Sign in with Apple, App Attest, App Store payments and refunds. Apple acts under its own privacy policy for these services. | United States, Ireland and other locations Apple uses |

We may also disclose data where the law requires it, for example to a court or a
public authority with a valid order.

**International transfers.** Using these providers transfers personal data
outside your country: to the EU (Supabase) and to the United States (Cloudflare,
RevenueCat, Apple). For each transfer we rely on
standard contracts under Article 9 of the KVKK, signed with each provider and
notified to the Turkish Personal Data Protection Authority, and, under the GDPR,
the European Commission's standard contractual clauses (or the EU–US Data
Privacy Framework where the provider is certified).

## 9. Your rights

Depending on where you live, you can:

- ask whether we process your personal data, and get a copy of it;
- have incorrect data corrected;
- have your data deleted;
- restrict or object to processing, including processing based on legitimate
  interest;
- receive data you gave us in a portable format;
- withdraw consent you gave (for example, turning off AI Capture in Settings →
  AI), without affecting processing before you withdrew it;
- object to a result that harms you and comes solely from automated processing;
- claim compensation if you are harmed by unlawful processing;
- complain to a data protection authority. In Türkiye this is the Personal Data
  Protection Authority (KVKK, kvkk.gov.tr); in the EU, the authority in the
  country where you live or work.

To use a right, email goralanil@gmail.com (ask by email for the postal address if you prefer to write). The Turkish
version of this policy explains the formal application methods under KVKK. We
answer free of charge within one month (30 days under KVKK). We may ask for
information to confirm the request is yours, but no more than we need.

Because your tasks are only on your device and we keep no AI Capture text, a
request about your data will usually only concern your account (identifiers
and email address), your plan and usage counter, any computer keys, the
RevenueCat customer record and, if you can identify it, an App Attest record.
It helps to write from the email address you use with Sign in with Apple, or to
tell us which one it is.

## 10. Security

Connections to our services are encrypted. AI Capture requests must carry Apple
App Attest proof. Only our own servers can read or change the account database.
Sign-in data on your device is kept in the iOS Keychain. No system
is perfectly secure, and your tasks are only as safe as your device: use a
passcode and keep iOS up to date.

## 11. Children

The app is not directed at children under 16, and we do
not knowingly process their personal data through the online services.

## 12. Changes

If we change this policy, we will update the effective date above, and tell you
in the app before a change that affects how your data is used takes effect.

## 13. Contact

Anil Goral, goralanil@gmail.com
