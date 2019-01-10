# trubb_CasualtyEndCondition

A quick and dirty way to end missions if there are too few players alive.

### How it works

At the start of the mission we count how many players are present, based on this count the current amount of alive players is continuously checked.  
The mission is ended when a side has fewer players alive than their treshold.

The maximal percentage of casualties is set through the variables `trubb_*_casualty_limit` in `initServer.sqf`. While these are technically editable during a mission I do not recommend changing them after mission start.

The variables `trubb_wait` and `trubb_mission_end` mustn't be edited. Considering a way to not have these publicly exposed to be implemented in the future.

### Adding this to your mission

1. Copy the contents of `description.ext` and `initServer.sqf` into the respective files in your mission folder.
2. Copy the folder `\functions` into your mission folder.
3. Edit the values assigned to the variables `trubb_*_casualty_limit` in `initServer.sqf` to your liking. **Do NOT remove them.**

That's it! Now you're done, but don't forget to inform your players.
