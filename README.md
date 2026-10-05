# ABES Attendance Tracker

A lightweight Chrome/Brave extension for **ABES Engineering College students** to sync and understand attendance from their own logged-in ABES ERP session.

**Current stable version:** v5.1.0  
**Developed by:** Rajnish Kumar — B.Tech CSE (Data Science), ABES Engineering College

## Features

- Syncs attendance from the student's currently logged-in ABES ERP session.
- Shows the **official ERP overall attendance percentage**.
- Subject-wise **Present, Absent, Total and attendance %**.
- 75% target calculator: tells you how many upcoming classes to attend.
- Shows how many classes can be missed while remaining at or above 75%.
- Date-wise attendance history.
- Supports **multiple lectures on the same date** and preserves ERP's lecture count.
- Saves the latest synced attendance locally for offline viewing.
- Works separately for each student's own browser/ERP session.
- Includes a one-click option to clear locally saved attendance.

## Installation

1. Open the **Latest Release**: https://github.com/rajneeshchaurasia47-ctrl/ABES-Attendance-Tracker/releases/latest
2. Download `ABES-Attendance-Tracker-v5.1.0.zip`.
3. Extract the ZIP to a permanent folder.
4. Open `chrome://extensions` in Chrome/Brave.
5. Turn on **Developer mode**.
6. Click **Load unpacked**.
7. Select the extracted folder that directly contains `manifest.json`.
8. Pin **ABES Attendance Tracker** from the Extensions menu.

## How to use

1. Log in to ABES ERP normally.
2. Open **My Attendance** in ERP.
3. Open the extension and click **Sync Now**.
4. Your latest attendance is saved locally and remains viewable until the next sync or until you clear it.
5. If the ERP session expires, log in to ERP again before syncing.

## How the 75% calculator works

For each subject, the extension uses the ERP's **Present** and **Total lecture** counts. If attendance is below 75%, it calculates the minimum consecutive classes required to reach 75%. If attendance is already at least 75%, it calculates how many upcoming classes can be missed while staying at or above 75%.

Date-wise history entries are not treated as lecture totals: one ERP history entry/date may represent multiple lectures.

## Privacy & security

- The extension **does not collect or store your ERP password or OTP**.
- It uses only the student's already authenticated ERP session when **Sync Now** is pressed.
- Attendance data is stored in Chrome's local extension storage on the user's own browser.
- No attendance data is intentionally sent to an external server by this project.
- Use **Clear saved attendance** to remove locally cached attendance.

See [PRIVACY_POLICY.md](PRIVACY_POLICY.md) for more information.

## Compatibility

Designed for the current ABES ERP student attendance page. If ABES changes its ERP page structure or attendance endpoints, a future extension update may be required.

## Release

Download the latest stable build from **Releases**:  
https://github.com/rajneeshchaurasia47-ctrl/ABES-Attendance-Tracker/releases/latest

## Disclaimer

This is an **independent student project** and is not an official ABES Engineering College application. ABES ERP and related names/services belong to their respective owners.

---

### Developer

**Rajnish Kumar**  
B.Tech CSE (Data Science)  
ABES Engineering College
