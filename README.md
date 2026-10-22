<!--
  The README for the public download repo github.com/ndmr0/aurator.
  Copy this file there as README.md on every release, after filling in
  "What is new" from CHANGELOG.md. The prices below are checked against
  site/lib/plans.ts by site/scripts/test-r3web-brand.mjs, so a price change
  on the site fails the tests until this file matches.
-->

# Aurator for macOS

Just talk, and it is written. Aurator turns your voice into clean text in every
app on your Mac, writes whole messages for you, and coaches you to speak better
from your own words. Private by default, cloud by choice.

Website: [tryaurator.app](https://tryaurator.app)

## Download

Get the latest version from [tryaurator.app/download](https://tryaurator.app/download),
or download [Aurator.dmg](https://raw.githubusercontent.com/ndmr0/aurator/main/Aurator.dmg)
from this repository. Open the file, drag Aurator into Applications, and open it.
It asks for the microphone, so it can hear you, and for Accessibility, so it can
type at your cursor.

Aurator is signed and notarised by Apple and updates itself. When a new version
is out, it asks you before it installs anything.

## Price and plans

Use everything free for seven days. Then pay once, in US dollars. There is no
subscription, and every plan includes every update.

| Plan | Price | Works on |
|---|---|---|
| One Mac | US$29 | one Mac |
| Three Macs | US$49 | up to three Macs |
| Every Mac | US$69 | every Mac signed in to your Apple account |

You can upgrade later and pay only the difference, and your key stays the same.
If Aurator is not right for you, ask within 30 days of a payment for a full
refund. The current prices are always on [tryaurator.app](https://tryaurator.app/#pricing),
and the [terms of sale](https://tryaurator.app/terms) explain refunds and upgrades.

## What you need

- macOS 26 or later, on a Mac with Apple silicon. Aurator is also built for
  Intel Macs, but it has not been tested on one yet, and Apple's on-device
  speech engine may not be available there, so dictation may need Cloud and
  your own Deepgram key. Please use the free week to check it before you buy.
- On Apple silicon, dictation, cleanup, the coach and the dictionary run on the
  Mac itself.
- Write for me, voice editing, the rewrite styles and building your voice on the
  Mac need Apple Intelligence, which needs a Mac with Apple silicon. Without it,
  those four work only with Cloud and your own Anthropic key.

## What is new in 2.12.0

- Notes. Record a call or a meeting, both sides or just your microphone, and
  get a transcript and a summary made on your Mac. Each side of a call finds
  its own language, so a call in English and Spanish is written in both. You
  can mute either side, ask about a note, and export it.
- The coach teaches with 18 short spoken lessons. You answer out loud, and
  your answer is measured against the lesson's goal.
- A Help page with 84 articles that work offline, a Keyboard Shortcuts window
  and a Report a bug button.
- Snippets, your dictionary in a file, and a choice of how long History keeps
  dictations.
- Notes' sound is kept in Apple Lossless and checked sample by sample before
  the original recording is removed. A private dictation made during a note is
  never kept in its sound, its copies or a backup.
- Known limits: at Stop, about 0.1 seconds of your microphone from just before
  the click can be missing from a note, and the first time Help opens it can
  pause for about 0.2 seconds.

## What is new in 2.11.1

- Aurator no longer quits when you tap the dictation key with a microphone
  whose sound format differs from the one before, such as the built-in
  microphone after EarPods.

## What is new in 2.11.0

- AI drafts wait for you. A rewrite style, a voice edit or Write for me shows
  its result first, and nothing goes into another app until you approve it.
- Text goes only into the app, window and field you were in when you started
  dictating. If anything else is in front, it is copied instead and a notice
  says so.
- Password fields are never listened to, and with secure typing on a
  dictation stays on your Mac and is not saved.
- Rewrites and edits are checked before they go in, so a dropped not, a
  changed number or an added date is refused.
- Your own clipboard comes back after each paste, and Aurator never empties
  it when macOS does not let it read it.
- A first-run guide, recordings about 50 times smaller, and your licence kept
  in the Keychain, signed by the server.

## Your privacy, in short

- By default your voice and your words stay on your Mac. Speech to text,
  cleanup and coaching all run there, and your dictations are never sent to us.
- Aurator goes online to check for updates, by reading the small update file in
  this repository, and about once a day to check your licence with
  tryaurator.app. The licence check sends your key, a random id for your Mac,
  your Mac's name, a one-way hash made from your Mac's hardware id and your key,
  a one-time number, and on the Every Mac plan a one-way hash of a private
  iCloud id. It never sends your dictations.
- Cloud is off until you turn it on in Settings with keys from your own
  accounts. Then Deepgram receives your audio and your dictionary words while you
  speak, and Claude, made by Anthropic, receives text for the rewrite styles,
  voice editing, Write for me and building your voice. Nothing is sent to us.
  When you save a Deepgram key, with Cloud on for every app or for one app by
  its rule, Aurator asks Deepgram once whether it accepts the key. That request
  carries only the key.
- A note records your microphone and, for a call, your Mac's sound, so it holds
  the other people's voices. Its sound, transcript and summary are made and kept
  on your Mac. Only its text can go to Claude, with Cloud on and your own key,
  and Aurator asks you first.
- The full list of what goes where is at [tryaurator.app/privacy](https://tryaurator.app/privacy).

## Help

Write to [hello@tryaurator.app](mailto:hello@tryaurator.app). If you lost your
licence key, [tryaurator.app/recover](https://tryaurator.app/recover) sends it
again to the email you paid with.

This repository holds only the signed app and its update feed. Aurator is made
by [ndmr.au](https://ndmr.au) in Queensland, Australia, and is not affiliated
with Apple.
