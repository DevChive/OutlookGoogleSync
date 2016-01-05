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
* 2.1.0 
    * Added LicenseHeader file to work with extension
    * Fixed spelling errors
    * GoogleCalendar.UpdateCalendarEntries() Move Event != NULL outside of If/Else statement to it's own If statement, and performing Recurrence.UpdateGoogleExceptions before handling events, or else all the exceptions inherit the updated timestamp of the parent recurring event.
