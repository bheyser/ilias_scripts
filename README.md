
# ILIAS scripts collection


## database fixing/migration scripts


### fixTestQuestionOrderingGaps.php

**GENERAL INFORMATION**
* This script can be used to repair question ordering sequences of tests configured with a fixed question sequence.
* Due to a bug in earlier ilias versions it might be possible that the question ordering got broken like described in the corresponding mantis report.
* Mantis Report: https://ilias.de/mantis/view.php?id=20382

**USAGE INSTRUCTIONS**
* Save this script to your ilias root directory and either call it with the browser or by using the command line interface instead.
* For using the web browser you need to login with an account having administrative privileges.
http://<your.ilias.domain>/<ilias_path>/fixTestQuestionOrderingGaps.php
* For using the command line interface change to the ilias root directory and call the script by using the following command. Make sure you made the script executable.
./fixTestQuestionOrderingGaps.php <adminUser> <adminPass> <iliasClientId>
* The script will report a success message when it finishs its tasks.
* If any php fatal error occurs due to exhausting any ressource restrictions, simply call the script again until it finishs with the success message.