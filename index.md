# Privacy Policy for TimeNeeded

**Last updated:** November 2, 2026

## 1. General Information
This Privacy Policy outlines how the **TimeNeeded** mobile application (hereinafter referred to as the "App"), developed by **Igor Nawojski** (hereinafter referred to as the "Developer"), handles user privacy. TimeNeeded is designed with a strict privacy-first, offline-first approach.

## 2. Zero Personal Data Collection
TimeNeeded does not collect, track, profile, transmit, or sell any personally identifiable information (PII), usage metrics, analytics, or behavioral data.
- The App requires no user account, registration, or sign-in.
- The App does not run third-party advertising SDKs, tracking pixels, or telemetry frameworks.
- The App does not transmit your personal tasks, timer entries, or usage habits to the Developer or any external server.

## 3. Local Data Storage & Retention
All content created or configured by the user (including task names, categories, timer history, completion timestamps, widget preferences, and custom color choices) is stored exclusively on the user's local device (using encrypted SQLite/Room storage).
- The Developer has no access to your stored data.
- Uninstalling the App or clearing its storage via Android System Settings permanently deletes all local application data.
- If Android Cloud Backup (Auto-Backup) is enabled on your device, an encrypted backup of local app data may be managed directly by your operating system and linked Google Account according to Google's standard backup terms.

## 4. In-App Purchases & Internet Access
The App declares the `android.permission.INTERNET` permission solely for communicating with the **Google Play Billing API**:
- **In-App Purchases:** The App offers optional premium visual themes ($0.75 each). Financial transactions, payment processing, fraud prevention, and purchase authentications are executed entirely by **Google LLC** through the Google Play Store.
- The Developer never accesses, receives, or stores your payment details, credit card numbers, or billing address.
- All payment data is handled in accordance with [Google's Privacy Policy](https://policies.google.com/privacy).
- Network connectivity is never used to transmit personal user content or timer statistics.

## 5. System Permissions & High-Risk Capabilities
To provide its core time-tracking, focus, and distraction-blocking capabilities, TimeNeeded requests specific system permissions, which operate strictly locally:

### A. Distraction Blocker & App Usage Access (`PACKAGE_USAGE_STATS` & `QUERY_ALL_PACKAGES`)
- **Purpose:** TimeNeeded includes an optional Distraction Blocker / Focus Mode feature allowing users to restrict access to chosen distracting applications while a timer or Pomodoro session is active.
- **How it is used:** The App queries the system locally and in real time to determine whether an application selected by the user as "blocked" has been brought to the foreground.
- **Strict Privacy Guarantee:** The App does **not** log, track, aggregate, or build a profile of your application usage history. App identification is evaluated purely in volatile local memory (RAM) to trigger the local blocking screen, and this data is never written to persistent logs or transmitted off the device.

### B. Overlay Display (`SYSTEM_ALERT_WINDOW`)
- **Purpose:** Used strictly to display the full-screen blocking notification (`BlockerActivity`) on top of restricted applications when a distraction block is triggered during an active focus session.

### C. Foreground Service (`FOREGROUND_SERVICE` & `FOREGROUND_SERVICE_SPECIAL_USE`)
- **Purpose:** Required to maintain accurate real-time timers, countdown clocks, and ongoing notifications when the App is minimized, running in the background, or when the device screen is turned off.

### D. Notifications (`POST_NOTIFICATIONS`, `POST_PROMOTED_NOTIFICATIONS` & `USE_FULL_SCREEN_INTENT`)
- **Purpose:** Used to display ongoing timer status in the notification shade, alert you when a timer/session has elapsed, and provide full-screen timer completion alerts even when the device is locked.

### E. Haptics (`VIBRATE`)
- **Purpose:** Used strictly for interactive tactile vibrations during UI touch events and alarm vibration patterns when timers finish.

## 6. Children's Privacy
Because TimeNeeded does not collect, store, or transmit any personal information, it complies fully with the Children's Online Privacy Protection Act (**COPPA**) and the General Data Protection Regulation (**GDPR**). The App is safe for users of all ages.

## 7. Third-Party Services
The only third-party service integrated into TimeNeeded is:
- **Google Play In-App Billing (Google LLC):** Used exclusively for managing theme purchase licenses and receipt validation. For more details on how Google processes transaction data, refer to [Google Privacy Policy](https://policies.google.com/privacy).

## 8. Changes to This Privacy Policy
If updates to TimeNeeded introduce new features that change how permissions or functionalities operate, this Privacy Policy will be revised accordingly. Any updates will be published on this page with a revised "Last updated" date.

## 9. Contact Us
If you have any questions or feedback regarding this Privacy Policy or TimeNeeded, please contact:

**Developer:** Igor Nawojski  
**Email:** igor.nawojski@gmail.com
