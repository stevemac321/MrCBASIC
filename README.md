# MrCBASIC
The best BASIC compiler found so far is the one from QB64.org.

You need to set the screen mode.  SCREEN 11 on the first line.

Mouse input needs to be refactored, mouse handling is more complex now.  I added a subroutine that gets the CHX, CHY, and B params. 

Mouse x,y coordinates need to be recalculated due to resolution differences.  Added sub GetCoords that prints the coords as you click:

REM To get coordinates, comment next line (GetXY), then uncomment the line after that (GetCoords)

REM Be sure to restore for normal use.  Uncomment out GetXY, comment out GetCoords

557 GetXY CHX, CHY

REM 560 GetCoords ' use this to run in a loop to determine mouse coordinates

Replaced delay loops with sleep calls.  5 second delay, or press any key to advance (after music finishes).Need to flush keys afterwards _KEYCLEAR.

Code references labels not in this source file, e.g. 5000 to 20000, perhaps meant to end program 

WAVE keyword does not seem to be supported, see line 114 (label 349)

Mr. C (orginal author) says that much of the graphics was generated by the MacPaint program.

