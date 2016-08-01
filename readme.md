## Outlook Google Calendar Sync (revX).

_The **revX** simply means, forked by Xeno Innovations and slightly modified to suit our needs._

This project is a fork from Outlook Google Calendar Sync which in turn is a fork from Outlook Google Calendar. Confused yet?  Well, don't be.

### Differences
Overall we LOVE the OGCS project and think they did a GREAT job with it. However there were some annoying things that we just couldn't get past such as Splash Screens and Message Boxes popping up telling us we're not connected to the Internet - _already know i'm disconnected, so go away!_

There is one other thing we didn't care for much, but it will have to stay and was the code formatting rules used in the project. No one is perfect & developers everywhere all argue that their's is most optimal. To minimize this we've included EditorConfig 


Overall we applaud you, Paul Woolcock! Thank you for your continued efforts on, Outlook Google Calendar Sync and making it so great.


## Original sources
* Current fork: <https://outlookgooglecalendarsync.codeplex.com/>
* Original fork: <https://outlookgooglesync.codeplex.com>


## Change Log
* 2.2.3.0
    * DJS:
        * **Program.cs** - Removed splash screen
        * **MainForm.cs** - Removed annoying message boxes. Author removed one finally too.
    * Notable Author Changes - *since last*:
        * Added extra logging
        * Added extra sync parameters
        * PayPal submissions include your email address
        * Enhanced error catching
        * Enhanced Outlook syncing
    * v2.2.3.0 - Alpha
        * **Enhancements**
        - Capture error when G revokes token.
        - Ability to filter O categories.
        - Give hint the sync summary is NOT the logfile.
        * **Bugfix**
        - Remember "custom O date format" setting.
        - Remember "description O->G only" setting.
        - Properly release O recurrence COM references.
        - Cater for difference in recurrence UNTIL values (ICS vs MS)
    * v2.2.2.0 - Alpha
        * **Enhancements**
        - Added "Auto Sync" menu to right-click. Includes options to delay next sync.
        - Sync timer code reorganised into class.
        - Don't delete reminders in O if not synced to G due to DND.
        - Improve button and tab background colours.
        - Catch COM / DLL exceptions.
        - Purge log files older than 30 days.
        - Improved handling of old IANA timezones (eg. Calcutta/Kolkata)
        - Improved display at >100% display magnification
        * Bugfix
        - Don't throw away Event after updating it
        - Don't show program in alt-tab when minimised to task tray
        - Handle pseudo all-day events (midnight to midnight times)
    * v2.2.1.0 - Alpha
        * **Enhancements**
        - Added DND time range for reminders in Google.
        - Improved exportToCSV functions.
        - Shift-click Sync button to force a compare of all items (not just if recently modified).
        * **Bugfix**
        - Retrieve original yearly recurrence outside of sync range.
        - Recalculate sync range on every sync, not just load/settings update.
        - G->O for recurrence exception not syncing.
        - Re-select the right Outlook calendar when re-connecting to Outlook.
        - Store OGCSlastModified as culture invariant date in Google.
    * v2.2.0.0 - Beta
        * **Enhancements Rolled in from Alphas**
        - Now supports 64bit Outlook.
        - Changed from using Startup menu shortcut to registry key.
        - Improved error handling during sync.
        - Mention OGCS in version update alert.
        - Handle API daily limit being exhausted.
        - Added option of subscribing for guaranteed API quota.
        - Added option to use Google calendar default notification.
        - "About" tab includes config file location.
        - "About" tab now shows location the executable is running from.
        - Show tray icon after MainForm initialised.
        - Get on initialising during splash screen.
        - Ignore Google events without basic attributes (eg start date)
        - Ultra-Fine logging level added.
        - Mask email addresses unless logging at Ultra-Fine level.
        - Handle MeetingItems as well as AppointmentItems.
        - Discard items without a date range.
        - Required permissions now include Google user ID.
        - Make proxy, push sync and start on startup take effect without saving.
        - New abort method to kill background sync.
        - Added links to TroubleShooting Help section.
        - Minimum of 10 mins sync interval.
* 2.1.0
    * Added LicenseHeader file to work with extension
    * Fixed spelling errors
    * GoogleCalendar.UpdateCalendarEntries() Move Event != NULL outside of If/Else statement to it's own If statement, and performing Recurrence.UpdateGoogleExceptions before handling events, or else all the exceptions inherit the updated timestamp of the parent recurring event.
