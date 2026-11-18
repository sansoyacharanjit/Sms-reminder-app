# SMS Reminder — Android project

Configured defaults: phone SIM, first SMS at selected date/time, then one repeat every 15 minutes, maximum 5 total sends, stop when that same number replies exactly `OK` (case-insensitive).

## Build
1. Install Android Studio on a computer.
2. Open this folder as an existing project.
3. Allow Gradle sync and install Android SDK 35 if prompted.
4. Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Install the generated APK on your Android phone.
6. On first launch, grant SMS permissions. Also allow exact alarms if Android asks.

## Important limitations / safety
- This is a starter project source, not a compiled or tested APK. It has not been run on your handset.
- Android and phone manufacturers can delay background alarms; exact delivery at the minute is not guaranteed.
- The app must remain installed; the phone must be powered on, have mobile service, and have an active SIM/SMS allowance.
- SMS_RECEIVED and SEND_SMS permissions are sensitive/restricted by Android and Google Play. This project is intended for personal sideload/testing; Play Store publication may be rejected without an eligible core use case.
- Incoming `OK` matching is based on the sender number. Some carriers may format sender IDs differently. Test with your own second phone before relying on it.
- The current starter version does not yet include editing/deleting reminders, dual-SIM selection, delivery reports, a contact picker, or a persistent history screen.
- Only message recipients who have agreed to receive reminders. Repeated unsolicited SMS can be treated as spam. Respect quiet hours and local laws.
