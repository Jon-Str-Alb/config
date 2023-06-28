installed linux mint
cloned klipper git
built tronxy firmware using instructions from Jeff's 3D corner and Tronxy wiki
installed klipper with mainsail ui
mainsail wouldn't run?
installed klipper with fluidd
removed mainsail config and references
added web ui port exceptions in firewall to allow web interface from other PC's
disabled some USB handler in linux that was not allowing MCU identification (from pinned comment in Klipper youtube video)
added MCU id successfully, web UI now working
the current printer.cfg is modified "printer-tronxy-xy-2-Pro-2020.cfg"
I may consider switching to the "printer-Konstantin.cfg", which is from 2021 and was included with the install
    instructions from Jeff's 3D Corner
Ran thru "configuration checks", stepper motors, heaters and endstops seem to be working
Ran pid calibration on extruder, updated pid values
Next step is to run through "slicers" document to set up Cura (or Slic3r) for Klipper
Configured start and end gcode in klipper, need to check variables
Variables OK
Configuring extruder
Since 16 microsteps seems to be the going number, I'm changing all steppers to 16
5/22/2022
Configured pressure advance for Klipper at 0.035

5/23/23
I reconfigured the pressure advance using the tuning tower at 0.1094

6/22/23
consider adding "square_corner_velocity" instead of print jerk?

6/28/23
all prints seem to be overextruding after klipper update,
    reverting extrusion variables in printer config to stock