# Kraken

## Overview
Welcome to the Kraken! 

Contained here are all files we had to author in order to operate the Kraken for our purpose. Kraken/Jubilee assembly and operation information can be found at on the [Jubilee Wiki](https://jubilee3d.com/index.php?title=Main_Page). 

## Folder structure
We connect to the Kraken through a hardwired wifi router. All code is uploaded directly to the robot through the computer terminal, and all operation is performed through terminal. To use the robot simply run "main.py" and it will pull from the appropriate files; just make sure they're all on the same level. 

Config.py contains all hardcoded movement parameters and physical object locations. These will change slightly between machines so should be checked.

Input.py is what the user will interact with. It will prompt through method creation and ask for all necessary variable information.

Lib.py contains all true method files. Based on the method selected through input the correct methods will be pulled from here. 

Main.py is our central method file. Run this to operate the machine; it will pull from all other files.

Test_files contains the two methods we used for reproducibility and accuracy testing of the pipette. They might be a good starting point to see how we constructed methods and communicate with both the Kraken and the pipette.

Important note: machine_interface.py needs to be on every level for the Kraken to function.

## Issues/Possible Bugs
Lib 16-43: lower case and upper case ranges may be recognized as unique when they should be viewed as identical. I think this has been fixed but good to keep an eye out.
Main 32-35: the final print summary is incomplete.

Other: the combined method (serial dilution + maldi spot) still has some pretty significant bugs. I have worked around this by carefully arranging my samples and just consecutively running SD then M but I am actively working on fixing this issue. Stay tuned for an update!

## Citations
For the Jubilee Project please cite:
    Vasquez, Joshua & Twigg-Smith, Hannah & O'Leary, Jasper & Peek, Nadya. (2020). Jubilee: An Extensible Machine for Multi-tool Fabrication. 1-13.             10.1145/3313831.3376425. 
    
For the Kraken code please cite:
    McCormack,M.&ElGhandour,K.(2022)Kraken(V1.0)[Source code]. github.com/mccormolly/Kraken
    
For the Kraken design please cite:
    *pending*
