---
title: Privacy Policy
permalink: /mipie/privacy-policy/
---

# Privacy Policy

**MiPie** — effective September 4, 2026

## Summary

**MiPie does not collect any information.** Every record stays on your device and is never transmitted to the developer. There is no server, no account, and no analytics.

The app does communicate with **Apple's map services** to draw the map and to give your records a neighborhood name. Section 5 explains exactly what is sent.

The sections below explain this in detail.

## 1. Information the app processes

To place your Wi-Fi connections on a map, MiPie processes the following:

| Information | When | Stored |
|---|---|---|
| Precise location coordinates (latitude, longitude) | Once, at the moment a record is created | Yes |
| Wi-Fi network name (SSID) | At the same moment | Yes |
| Wi-Fi security type | At the same moment | Yes |
| Wi-Fi access point identifier (BSSID) | At the same moment | Yes |
| Time of the record | At the same moment | Yes |
| Administrative region (country, city, neighborhood) | **Just after** the record is saved | Yes |
| Name you give a record | When you type it | Yes |
| Travel speed | At the moment of the decision | **No** — used only to decide whether you are in motion, then discarded |
| Location accuracy | At the moment of the decision | **No** — used only to decide whether the fix is precise enough to record, then discarded |
| Recent activity history (walking, automotive, etc. — last 3 minutes) | At the moment of the decision | **No** — used only to decide whether you were recently in a vehicle, then discarded |

**The security type is stored** so that **open networks — those needing no password or login — can be excluded from your records.** Networks you join automatically on the street or on public transit would otherwise pile up and make the records meaningless. Security type describes the kind of network (open / password / login) and is **not the password itself.**

**The BSSID is stored** so that **moving access points can be filtered out.** Wi-Fi on a bus or train reappears with the same name and the same access point several kilometers away. If the same access point is seen more than 500 m from where it was recorded, the app treats it as something other than a fixed place and **deletes that record automatically.** This value is never shown on screen.

**The administrative region is stored** to label records with a neighborhood name and to award regional badges. It is derived from the coordinates; section 5 explains how.

The app does not track your location continuously. It takes a single location reading only while the app is on screen, and only at the moment a record is created. It does nothing in the background.

Activity history is likewise **not monitored continuously.** At the moment the app decides whether to record, it reads the last three minutes that your device has already accumulated, once, and then discards it.

## 2. Purpose

**One purpose only: showing your records on a map.** The information is not used for anything else.

## 3. Storage and retention

Records are stored solely in your device's local storage (Apple SwiftData).

- They are never transmitted to the developer's server (the developer runs none)
- No account is created and there is no sign-in
- No synchronization of any kind, including iCloud
- **Deleting the app deletes every record, with no way to recover them**

## 4. Sharing with third parties

**None.** MiPie contains no third-party SDKs of any kind, including analytics tools, advertising networks, and crash reporters. Your information is never sold or shared.

## 5. About Apple's map services

The app communicates with Apple's map services for **two reasons.** Both are governed by Apple's privacy policy.

**1) Map tiles** — downloaded to draw the map on screen.

**2) Turning coordinates into a neighborhood name** — to label a record as, say, `San Francisco, CA` and to award regional badges, **the record's coordinates are sent to Apple's reverse-geocoding service.** This happens once just after a record is saved, and again when the app retries records that have not yet been labeled. The result (country, city, neighborhood) is stored on your device, and **once stored the app never asks again for that record.**

**Network names are never included in this request.** Only coordinates are sent.

The app never sends your records **to the developer.**

## 6. About location permission

MiPie requests "While Using the App" location access with **Precise Location**. It never requests "Always" access.

Precise Location is required for two reasons:

1. Records need accurate coordinates to be meaningful on a map
2. **iOS discloses the Wi-Fi network name only to apps that have been granted Precise Location.** This is Apple's condition. With Precise Location turned off, the app cannot read the network name and the recording feature does not work

## 7. About Motion & Fitness permission

MiPie requests **Motion & Fitness** permission so that rides on a bus or subway do not turn into records.

Speed alone cannot catch a bus stopped at a light, because at that moment the speed is near zero. So, at the moment it decides whether to record, the app reads **the last three minutes of activity history your device has already accumulated** (walking, running, cycling, automotive) once, to see whether you were recently in a vehicle. What it reads is used for that decision only and is **never stored.**

**If you deny this permission, no records are created,** because there is no way to tell whether you are in a vehicle. The button at the bottom of the map says so and becomes a shortcut to Settings. The app **never monitors** your activity continuously.

## 8. About Wi-Fi passwords

**MiPie never asks for, reads, or stores Wi-Fi passwords.** The app does not connect you to any network. It reads only the **name, security type, and access point identifier (BSSID)** of the network you are already connected to.

## 9. Something you should know

Wi-Fi names combined with locations accumulate into a history of **where you were and when**.

These records never reach the developer (see section 5 for the coordinates sent to obtain a neighborhood name), but **anyone who can unlock your device can see them.** We recommend setting a device passcode along with Face ID or Touch ID.

## 10. Your rights

- **Delete individually**: You can remove records one at a time by tapping them on the map
- **Rename**: You can edit the name of any record
- **Delete everything**: Deleting the app immediately removes all records
- **Withdraw permission**: You can turn off access at any time in iOS Settings ▸ Privacy & Security —
  location under **Location Services**, activity history under **Motion & Fitness**
- Because the app keeps no information on any server, there is nothing to request access to or deletion of from the developer

## 11. Children's privacy

MiPie is not directed at children and does not knowingly process children's personal information.

## 12. Changes to this policy

Changes will be communicated through app updates and this document. In particular, if a change ever causes data to leave your device — synchronization, backup, analytics, or anything similar — we will give notice in advance and update the App Store privacy disclosure accordingly.

## 13. Contact

junchoia25@gmail.com

---

*This document describes how the app actually behaves. It is not legal advice.*
