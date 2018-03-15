# gsuite-ghome-cal
Gsuite/Google Home Calendar Integration

Follow these steps:

* Create a Calendar called "Work" in your personal account.
* Go to the "Settings" for this calendar:
  * Under "Share with specific people", add your Gsuite email address with "Make changes to Events" permission.
  * Copy the "Calendar ID" and paste in the script.
* Go to your Gsuite account and create a new AppScript: https://script.google.com/intro
* Paste the code from CalendarSyncGoogleHome.appscript into the new script.
  * Change the following:
    * Replace "gsuite-email" with your Gsuite Email.
    * Replace "personal-email" with your email on the Google Home account.
    * Replace "calendar-id-for-personal-calendar-from-settings" with Calendar ID copied above.
* Save the script.
* Click on Triggers for current project (Clock icon). Add a new Trigger to run the script every 6 hours or so.
* Try running the script manually. You should see events being copied from your Gsuite primary calendar to the Work calendar in your personal account.
* At the end of the run, the script will also send you an email to your personal email address with the status of the run.
* The script copies events for 7 days starting today and is safe to run multiple times.
* Note: The script will delete all events in the "Work" calendar in your personal account. So make sure to use this calendar only with this script.
* In your Google Assistant app select "Work" calendar under "Calendars" in Settings.

Based on: [https://github.com/prashantkhurana/GSuite_Calendar_To_Personal](https://github.com/prashantkhurana/GSuite_Calendar_To_Personal)
