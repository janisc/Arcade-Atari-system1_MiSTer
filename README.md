# Atari System-1 FPGA Arcade  

## About  
FPGA implementation of Atari's System 1 (LSI version) arcade platform from 1984.  
Based primarily on the SP-280, SP-286 schematics with additional support from SP-277, SP-298  

System-1 supported game cartridges according to MAME  
* Marble Madness (1984)  
* Peter Pack Rat (1985)  
* Road Runner (1985)  
* Indiana Jones and the Temple of Doom (1985)  
* RoadBlasters (1987)  

## Known Issues  
The following mra files don't work as expected.
* Indiana Jones (cocktail).mra graphics tiles incorrectly offset, directional controls not working.
* Indiana Jones (set 3).mra upside down corrupt or missing graphics, text is OK.

## Marble Madness controls  
* Marble Speed sets how far the marble moves for a given mouse/trackball or analog stick movement. 2:1 and 4:1 move it further for the same roll and suit trackballs that send few counts per revolution.  
* Marble Control selects player 1's input. With Mouse+Analog both are read, and a resting analog stick that is not quite centered can nudge the marble and make it hard to enter initials with a trackball. Mouse only ignores player 1's analog stick, Analog only ignores the mouse. Player 2 always uses the right analog stick of the first controller.  

## Building  
The project files are setup for Quartus 17  
