---
layout: default
title: "Privacy Policy for Windows and Mac – Eisenhower AI"
lang: en
---

# Eisenhower AI for Windows and Mac: Privacy Policy

Effective 29 October 2026.

This policy covers the Eisenhower AI desktop app for Windows and macOS. The
Windows app is distributed through the Microsoft Store and GitHub, and the Mac
app as a download from GitHub. The app is published by Anil Goral as Matrix
Solution. This policy is published at
<https://anilgoral.github.io/eisenhower-ai-legal/desktop-privacy/>. Questions:
<https://anilgoral.github.io/eisenhower-ai-legal/support/>.

## The short version

Your tasks stay on your computer. The app has no analytics, no telemetry and no
crash reporting. Apart from a check for a newer version, it sends nothing
anywhere until you turn on a feature that needs the internet. Those features
are listed below.

## What stays on your computer

- **Your tasks.** Each task is a Markdown file in a folder you choose. By
  default it is `Eisenhower AI` in your Documents folder (on Windows, the
  OneDrive Documents folder if OneDrive manages it). If that folder is synced,
  for example by OneDrive or iCloud, your sync provider handles it under its
  own terms.
- **Backups.** One zip of your task folder a day, the seven newest kept, in the
  app's own data folder. You can turn this off in Settings.
- **Settings and logs.** Preferences, the list of folders you opened, and a
  small log of the app's own errors. The log is not designed to hold task text,
  and it never leaves your computer. "Copy error report" copies a report to
  your clipboard for you to send if you choose.
- **Reminders.** Reminders are shown by your computer's own notifications.
  Nothing about them is sent anywhere.
- **Keys and sign-in details.** AI keys you enter, and the device key that
  signs you in to Eisenhower Pro, are kept in Windows Credential Manager or,
  on a Mac, in the Keychain. The app's window only ever sees a masked copy of
  an AI key.

## Checking for a newer version

About 15 seconds after it opens, the app asks GitHub whether a newer version
exists, by downloading a small file from github.com. The request carries no
account, task or device identifier; GitHub sees your IP address, as it would
for any web request. If there is a newer version, the app offers "Restart to
update", and only if you click it does it download the update, also from
GitHub. The update is checked against our signature before it is installed.
Without an internet connection the check simply fails, silently. The
Microsoft Store version never makes this check: the Store updates it.

## Features that use the internet, and only when you use them

**AI sorting with your own key.** If you choose Google Gemini, OpenAI,
Anthropic or Groq and save your API key, the text you type into AI Capture is
sent to that provider when you press Classify. Saved tasks, notes and your task
folder are not sent. The provider processes the text under its own terms and
privacy policy, using your key. Requests to OpenAI ask it not to store them.

**Local AI.** If you choose Local AI, the text goes to a model running on your
own computer (LM Studio, at 127.0.0.1). The app refuses any address that is
not on this computer.

**Eisenhower Pro.** Pro is an optional paid account shared with the Eisenhower
AI iPhone app, and it is handled as described in that
[privacy policy](https://anilgoral.github.io/eisenhower-ai-legal/privacy/). On
this computer:

- **Signing up or in** sends your email address and password to the account
  service (Supabase). The password is not stored on your computer. Sign in
  with Apple opens your browser and returns to the app.
- **Each sign-in** registers a key for this computer. The app then proves who
  you are with a signature, without a password, and checks your subscription
  each time it starts.
- **AI Capture with Pro** sends the text you typed, with your language and
  time zone, to our own AI service. No other AI company receives it.
- **Subscribing and managing your subscription** open RevenueCat's or Apple's
  pages in your browser. The payment is handled there, outside the app and
  outside the Microsoft Store.
- **Signing out** removes this computer's key from your account and deletes
  the sign-in details from Credential Manager or the Keychain. To delete your
  account, see the Pro privacy policy.

**Voice input on Windows.** Speech is turned into text on your computer, by a
speech model the app downloads once (190 MB, from Hugging Face, which sees an
ordinary download request and nothing about you). The microphone records only
between pressing Mic and pressing Stop, for at most two minutes. The audio
stays in memory until it is transcribed, and is never stored or sent anywhere.
Only the resulting text reaches the capture box.

**Voice input on a Mac.** Speech is turned into text by macOS's own speech
recognition, which may send the audio to Apple to do so, under Apple's privacy
policy. The first time, macOS asks whether the app may use the microphone and
speech recognition; you can change either answer later in System Settings >
Privacy & Security. The app receives only the resulting text, and does not
store or send the audio itself.

## What we do not do

We do not sell personal information, show ads or track you across apps or
websites. The app does not collect your contacts, location or files beyond the
task folder you choose.

## Your choices

- You can use the app offline with AI turned off. Only the check for a newer
  version then tries to reach the internet, and the app works the same when it
  cannot.
- You can delete AI keys in Settings, sign out of Pro, and turn backups off.
- What uninstalling removes depends on where the app came from. Your task
  folder is never touched.
  - **Microsoft Store:** backups and logs are deleted. Settings stay in
    `%LOCALAPPDATA%\com.eisenhowerai.next`, and saved keys in Credential
    Manager; remove keys in Settings before uninstalling, or in Credential
    Manager afterwards.
  - **Windows, from GitHub:** saved keys, logs and the speech model are
    deleted. Backups and settings stay in
    `%LOCALAPPDATA%\com.eisenhowerai.next`, in case your task folder is ever
    lost, and you can delete that folder.
  - **Mac:** moving the app to the Trash removes nothing else. Backups stay
    in `~/Library/Application Support/com.eisenhowerai.next`, settings in
    `~/Library/WebKit/com.eisenhowerai.next`, logs in
    `~/Library/Logs/com.eisenhowerai.next`, and saved keys in the Keychain.
    Remove keys in Settings first, then delete those folders.

## Changes

If this policy changes, the new version will be published at the address above
and with the app's Store listing, with a new effective date.
