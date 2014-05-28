ee-attenee-import-modified
==========================

This is a modification to Event Espresso's Attendee Import plugin, adding a loop to import custom questions from a csv file

It is not endorsed or supported by Event Espresso - use at your own risk!





In the array starting on line 219 we added additional data fields to be inserted into the EVENTS_ATTENDEE_TABLE using the syntax 'value' => $strings[Z] with Z being the column number containing the data in the csv file.

At line 268 we added additional data to the EVENTS_ANSWER_TABLE using the following syntax 						

case X :
$answer = $strings[Z];

where X is the Event Espresso question number and Z is the column number containing the answer in the csv file

