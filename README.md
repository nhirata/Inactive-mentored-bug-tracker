# IMBT

To run the script enter the pertinent information into login_info.py and run inactive_mentored_bugs_tracker.py live from the command line.

If you want to do a dry run where the script will only find the bugs and print relavent information about them then run inactive_mentored_bug_tracker.py dry_run from the command line.

Due to the nature of the bzrest library used this is not python 3 compatible.

This is in response to mozilla bugzilla bug 1128878 (https://bugzilla.mozilla.org/show_bug.cgi?id=1128878) requested by Josh Matthews quoted below 

It's common to find mentored bugs that have been assigned to a contributor weeks or months ago, with no subsequent followup from the assignee. This is currently handled on an ad-hoc basis; I propose writing a tool that will perform the following steps:

* find the set of mentored bugs with an assignee where the last modified date is >3 weeks
* Set the assignee back to default (nobody@mozilla.org)
* ~~Request needinfo? from the previous assignee~~
* Leave a comment like "I have reset the assignee as part of an automated cleanup since there has been no visible activity in this bug for some time. If this is incorrect, please leave a comment to let me know and I'll correct the error."
