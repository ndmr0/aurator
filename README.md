<!--
  The README for the public download repo github.com/ndmr0/aurator.
  Copy this file there as README.md on every release, after filling in
  "What is new" from CHANGELOG.md. The prices below are checked against
  site/lib/plans.ts by site/scripts/test-r3web-brand.mjs, so a price change
  on the site fails the tests until this file matches.
-->

# Aurator for macOS

Just talk, and it is written. Aurator turns your voice into clean text in every
app on your Mac, writes whole messages in your voice, and coaches you to speak
better from your own words. Private by default, cloud by choice.

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
  Intel Macs, but it has not been tested on one yet, so on an Intel Mac please
  use the free week to check that dictation works before you buy.
- Dictation, cleanup, the coach and the dictionary run on the Mac itself.
- Write for me, voice editing, the rewrite styles and building your voice on the
  Mac need Apple Intelligence, which needs a Mac with Apple silicon. Without it,
  those four work only with Cloud and your own Anthropic key.

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
  When you choose Cloud and save a Deepgram key, Aurator asks Deepgram once
  whether it accepts the key. That request carries only the key.
- The full list of what goes where is at [tryaurator.app/privacy](https://tryaurator.app/privacy).

## Help

Write to [hello@tryaurator.app](mailto:hello@tryaurator.app). If you lost your
licence key, [tryaurator.app/recover](https://tryaurator.app/recover) sends it
again to the email you paid with.

This repository holds only the signed app and its update feed. Aurator is made
by [ndmr.au](https://ndmr.au) in Queensland, Australia, and is not affiliated
with Apple.
