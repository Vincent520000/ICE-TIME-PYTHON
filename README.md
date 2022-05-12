# ICE-TIME-PYTHON
A statistician meticulously records the names of players, the period, the time on the clock when a player stepped on the ice and the time when a player stepped off the ice. They then record this in a comma separated values file format (CSV file) such as the following file (call this example ice_times.txt):

Zoe Son,1,20:00,19:00
Wayne Gretzky,1,20:00,19:23
Mark Messier,1,20:00,18:53
Hayley Wickenheiser,1,18:53,17:00
Wayne Gretzky,1,1:00,0:00

You may assume periods will be 1, 2 or 3, that names are unique for players (so teams can only have one person named 'Wayne Gretzky'), that names do not contain commas and that times will not overlap for a player. The last line in the file may or may not end with a newline character.

Write a function

ice_times(filename_in, filename_out)
         
which consumes two strings filename_in, corresponding to the non-empty CSV file created in the above format and a string filename_out that is the output file name, returns None and writes to the file name in filename_out the number of seconds each player played in the following CSV format:

Name1,seconds
Name2,seconds
...
where each line ends in a newline character (including the last) and the names are in alphabetical order.
