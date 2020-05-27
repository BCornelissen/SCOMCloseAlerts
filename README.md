# SCOMCloseAlerts
Scripts to help close alerts in SCOM coming from Rules

This small PowerShell script was created to close old alerts coming from rules in SCOM 2012. Alerts from rules do not auto-close so you will have to manually close them. This script looks for those alerts and specifically also checks for the last modified date (and not the alert age). If it was not modified since the last X hours (you define X first in this script, else it is 96 hours by default) it will close those alerts for you and insert a comment. This can help to clean up some environments of a lot of old alerts which are still open. Or you could just schedule this script to run.

More information can be found on https://blog.topqore.com/scom-2012-close-old-alerts/

The other script was for SCOM 2007 R2 and does the same. Had to find a place for it when Technet Galleries was closing down.
