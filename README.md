# Full-GC-Controller
Unlike other GC controller projects, this project focuses on making the Arduino act as a robust controller (instead of simply reading a controller)

# Intro
This project is meant to make the Arduino output Gamecube controller signals rather than the more common applications of reading from a GC controller.

Ultimately, my plan is to make the Arduino record inputs from a GC controller then replay them with precise timing, for use in particularly Sm4sh Wii U. This feature may or may not end up in this repo, but ultimately I'll be making a more extensive Sm4sh controller utilizing this library in a different repo once this project works well.

Note that this project initially used the Arduino Due, but due to various reasons, the Arduino Uno is now being used. Thus, the "Legacy (Due) Code" contains the deprecated (and not fully functional) Due code that may be visited at some point in the future.

# Goals
 * Arduino is able to read commands from a console (such as probing for controller or request for data)
 * Arduino is able to send a properly formatted of data as requested (ie, all the buttons feedback)
 * Code is packaged into an "easy" to use library (or at least functions) for reading and sending data. Includes easy way to read and write single bits as well as send entire controller commands with ease (ie, without delving into the library at all)
 * Code is robust and works well with as many minimized timing glitches as possible, with as little timing hardcoding/assembly as possible
 * Stretch goal: Be able to easily record inputs from a controller (so the Arduino will be able to act as a console)
 * Stretch goal: Be able to fairly **easily** (with as little complex "user"-level code as possible) have the Arduino output fairly complex GC controller sequences

# Tools used
Noted here in case my setup doesn't work with other applications. If you notice a case where the setup doesn't work, please let me know by creating an issue!
 * Arduino Uno
 * Wii U GC Adapter
 * Windows 10 PC + [Massive's GC USB Driver + vJoy Monitor](http://m4sv.com/page/wii-u-gcn-usb-driver)

# Current Status: WIP/Not yet done or even satisfactory
Please visit the readme within the "Current (Uno) Code" folder for a more up to date and better description.

# Side Notes
If anyone would like to port the code to Due or otherwise help make the code more universal (such as by simply pointing out a more universal yet still all together correct method of doing something), I would highly appreciate it!

----------------
# Readme Todos
 * Add description of circuit plus how to recreate it (eg, plus pull-up resistor console vs controller)
 * Add description of communication protocol from my perspective
 * Add useful sources
 * Probably create a wiki very soon instead and move much of this over there
