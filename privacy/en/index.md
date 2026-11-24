---
title: Privacy policy — BTW
lang: en
---

# BTW privacy policy

Effective November 24, 2026 · [Русская версия](../)

BTW — Buy The Way (called «Сусеки» in the Russian interface) is a shared family shopping list. The app has no server and no accounts of its own: what you enter is stored on your phone and, if you turn on sync, on your own Synology NAS. The developer does not receive, collect or store your data.

## Which versions this policy covers

This policy covers every version of the BTW / «Сусеки» app (Android package `org.koda.shopping`), however you installed it:

- **RuStore** — installed from the RuStore app store;
- **GitHub** — the APK file from the project's GitHub releases page;
- **iPhone** — the iOS version.

The versions differ only in how they are updated (see "Third-party components and updates"); all of them handle your data the same way.

## Data the app processes

| Data | Why | Where it is stored |
|---|---|---|
| Lists, items, "bought" marks, change history | The core feature | On the phone; with sync, on your NAS |
| Family name, mark colour, grammatical gender (Russian verb forms), profile photo (optional) | Showing family members who added and bought what | On the phone; with sync, on your NAS |
| NAS address, QuickConnect ID, DSM login and password, trusted-device token (2FA), trusted certificate fingerprints | Connecting to your NAS | Only on the phone, in the encrypted system store (Android Keystore / iOS Keychain); excluded from backups |
| Random install identifier | Telling this phone's files from other family devices' files on the NAS | On the phone and in file names on your NAS |
| Voice (only while you dictate) | Voice input of items | The app does not record or store audio, see below |

The app does not collect location, contacts or advertising identifiers and shows no ads.

## Sync with a Synology NAS

Sync is optional: without it the app works on one phone only. When you connect a NAS, the app talks to it directly (on your local network or over the internet) and keeps its files in the "Shopping List" folder of the DSM user's home folder. Everyone who signs in with that DSM account — usually your family — can access these files. The app does not create DSM accounts.

If you enter a QuickConnect ID, the app asks Synology's QuickConnect service (global.quickconnect.to) for your NAS address and, when needed, connects through its relay. NAS discovery on the local network uses mDNS/Bonjour and stays within your network.

## Voice input

Speech is recognised by the phone's system service, not by the app. On iPhone recognition runs on the device when supported; otherwise Apple processes the recording. On Android the recogniser chosen in the system (usually Google or Yandex) does the work; depending on the device and settings, audio may be sent to that service. The app receives only text. You may decline microphone access; everything else keeps working.

## Camera and photos

You choose a profile photo yourself, from the camera or the gallery. The app receives only the selected image.

## Third-party components and updates

- **The RuStore build** uses the RuStore In-app Updates SDK (VK LLC) to check for and install updates. The SDK includes RuStore analytics and metrics modules that may send technical data about the update flow and the device to RuStore; see the [RuStore policy](https://www.rustore.ru/help/legal/).
- **The GitHub build** checks GitHub (github.com) for updates; like any web server, GitHub sees the phone's IP address.
- **The iPhone version** does not check for updates itself.

There are no other SDKs (analytics, ads, crash reporting) in the app.

## Retention and deletion

Data is kept until you delete it. Deleted items are marked deleted and disappear from the sync files after about 30 days; the change history on the phone is kept for 7 days.

- To delete data from the phone, uninstall the app or clear its data in system settings.
- "Sign out of DSM" in the profile removes the login and password from the phone; "Forget" next to "This phone is remembered" removes the trusted-device token.
- To delete data on the NAS, delete the "Shopping List" folder in File Station.

## Children

The app is not directed at children and collects no age data.

## Changes

A new version is published on this page with a new date at the top.

## Contact

Questions about the app or this policy: [shoppingapp@list.ru](mailto:shoppingapp@list.ru)
