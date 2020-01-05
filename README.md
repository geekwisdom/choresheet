# Famliy Choresheets

> There is no daily chore so trivial that it cannot be made important by skipping it two days running. —Robert Brault

In our family we all take responsibility for household chores. This tool regularily prints 
a different choresheet each week, rotating the chores among famliy members


## Getting Started

Extract the github project to a location on your linux box (eg: /usr/local/scripts/autoprint)

Modify the chorelist ods (Open Office 'Calc' File). Unless perhaps your family
happens to have the same names as mine. Extract each rotating week as a 
diffeent PDF in the format of "ChoreSheet{X}.pdf" where X is 1, 2 ,3 4 etc

Schedule a cronjob on a weekly basis. Each week a new ChoreSheet{X} file is printed to your printer

use the prarameter 'reprint' to repring the last sheet manually without 
impacting the current sheet.

*Note: This script writes the last chorenum by default to your $TEMP directory.
On many linux machines this folder is erased on each reboot, so your chore
count will restart at 1 with every restart. To prevent this point the location to a different folder

