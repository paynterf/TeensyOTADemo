# TeensyOTADemo
 Teensy OTA Update Demo
 
 This Teensy sketch demonstrates the technique for 'over-the-air' (OTA)
 updates of Teensy sketches, using the Microsoft VS2019 IDE with the 
 Visual Micro extension.
 
 This demo program does nothing but flash the built-in LED.  However,
 it incorporates Joe Pasquariello's 'FlasherX', so it supports OTA flash
 operations.  
 
 To use this program, make sure that 'board.txt' is in the same folder,
and that the OTA serial port is selected, and that the companion 'TeensyFlash'
command-line program is in a reachable location.  When the sketch is compiled in 
Visual Studio 2019 with the Visual Micro extension, the command in 'board.txt'
runs as a post-build command and launches 'TeensyFlash' with arguments specifying
where the .HEX file can be found and which COM port to use to communicate with the 
Teensy at the other end of the OTA link.
