# -TES3MP-Morrowind-Rebirth-Gates-Fixed
This is my take on fixing Morrowind Rebirth gates behaviour for 0.7 alpha TES3MP.
It also is pretty customizable.

## Installation

1. Download the ```Morrowind Rebirth TES3MP Gates.esp``` and load it AFTER ```Morrowind Rebirth [Main].esp```

What this esp does is: 

a) remove original gate script from affected gates; 

b) replace it with custom one (edited version of original to fit the needs of TES3MP)
                        
         
2. Download the ```main.lua``` from ```MR_Rebirth_Gates``` folder and put it in */server/scripts/custom/MR_Rebirth_Gates/*
3. Open ```customScripts.lua``` and add this code on separate line: ```require("custom/MR_Rebirth_Gates/main")```

## Description

I wanted to play Morrowind Rebirth. Was looking forward to the day/night cycle of certain gates. I bumped into problem where one wing of gate would disappear at night (at least in Balmora) making the lock on the door useless. 

[CLICK THE PICTURE FOR REFERENCE - YT VIDEO][![For reference see:](https://img.youtube.com/vi/LNbxP7jFMrM/maxresdefault.jpg)](https://youtube.com/watch?v=LNbxP7jFMrM)

[CLICK THE PICTURE FOR SHOWCASE OF THE FIX - YT VIDEO][![Showcasing the fix:](https://img.youtube.com/vi/Ws6H7ahT4QQ/maxresdefault.jpg)](https://youtu.be/Ws6H7ahT4QQ)



## Configurables

scriptConfig.openGatesOnDaytime = true 
-- when the hour shifts to 6 a.m. the city gates will open, else will only unlock (Default: true)

scriptConfig.lockLevelDay = 1000 
-- so players can't use the door (using OnObjectActivate would be safer approach)

scriptConfig.lockLevelNight = 100

scriptConfig.createTimerCountdown = 1000 
-- in miliseconds -> Default: 1 second (1000)

scriptConfig.resetTimerCountdown = 1000 
-- in miliseconds -> Default: 1 second (1000)

scriptConfig.lockedGateStart = 22 
-- hour when the gate gets closed and locked

scriptConfig.lockedGateEnd = 6 
-- hour when the gate gets unlocked again

## Credits

Of course to the original creator of Morrowind Rebirth - Trancemaster.



