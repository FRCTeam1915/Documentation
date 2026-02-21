### 1. Machine Overview

The Boss laser model LS2440 is a high-powered CO2 laser used for prototyping and building robot components in the FIRST Robotics program. It is primarily used for cutting materials such as cardboard, wood (HDF, plywood) and acrylic (plexiglass). The machine supports cutting of organic and non-metal materials. It features a 150W laser power and a cutting area of 39.75" x 23.6". The laser head includes auto-focus and air-assist capabilities, and it has a motorized Z-table with a working height of 7 inches.

### 2. Safety Information

The Boss laser is classified as a Class 4 laser, which poses serious eye and skin hazards. Laser safety goggles are typically required, they are not needed when the laser hood is properly down. Users must follow strict safety protocols including proper ventilation and equipment setup. The machine has built-in safety features such as an illuminated LCD panel for control and an inline beam combiner for improved accuracy. Emergency procedures include immediate shutdown and contacting a mentor if any malfunction occurs. Training on safe operation is required before using the machine.

### 3. Materials

IF IT ISNT IN THE LIBRARY ASK A MENTOR BEFORE YOU CUT

Acceptable Materials
- Wood
- Acrylic
- Cardboard
- Paperboard
- Corrugated Plastic
- MDF
- HDF
- Magnetic Sheets
- Nylon

Banned Materials (These materials either wont cut or will produce toxic fumes)
- PVC (Polyvinyl Chloride) and Vinyl: Release toxic chlorine gas and hydrochloric acid fumes when heated, which can corrode laser optics and endanger operators. 
- ABS (Acrylonitrile Butadiene Styrene): Melts and burns, releasing cyanide gas, a highly toxic substance, and creates a sticky, difficult-to-clean residue. 
- Polycarbonate: Highly flammable and can release hazardous fumes; thick sheets are especially dangerous and may cause fires. 
- Fiberglass: Contains resins that emit toxic fumes (e.g., formaldehyde, acrolein) and releases fine glass particles when cut. 
- Carbon Fiber: Produces hazardous fumes (including cyanide) due to epoxy resins and can cause delamination and damage optics. 
- Foam and Styrofoam: Highly flammable and release toxic gases like styrene and hydrogen bromide when heated.  
- PTFE (Teflon): Releases fluorine-based toxic fumes when cut. 
- Halogens and Halogenated Compounds: Found in some plastics, fire retardants, and cleaning agents, they release harmful gases when heated.
- Metals

### 4. Proper Use

To properly operate the Boss laser, follow these step-by-step procedures:

1. Ensure the bed is empty and the laser nozzle will not hit anything if it moves completely to the far right.

2. Turn the key located above the control panel to power on the laser. The machine will automatically home, so be prepared for movement.

3. Flip the switch on the front of the white box on the floor to the right of the laser to turn on the cooler.
⚠ THE COOLER MUST BEEP BEFORE PROCEEDING.

4. Flip the wall-mounted power switch on the left side of the laser to turn on the air assist and exhaust. This may be turned on later to reduce noise, but it MUST be on before cutting.
⚠ THE EXHAUST AND AIR ASSIST ARE LOUD. IF YOU DO NOT HEAR THEM, THEY MUST BE FIXED BEFORE RUNNING THE LASER.

5. Load the material onto the cutting bed.
   - If the material is too small for the slats, place the mesh bed (located to the left of the laser) on top of the cutting bed.
   - If the material is too large to fit:
     • Open the back and side panels using the center latch.
     • Keep the latch closed while the door is open so the material can lay flat.
     • Remove the front panel by pulling the latches located inside the hollow bar on either side.

6. Adjust the Z-height using the control panel for optimal cutting depth (using either Auto Focus or the leveling guide).
⚠ THE NOZZLE MUST MOVE FREELY UP AND DOWN BEFORE USING AUTO FOCUS.
⚠ DO NOT USE AUTO FOCUS ON WEAK MATERIAL (IF A PENCIL CAN EASILY PUNCTURE IT). THE NOZZLE CAN AND WILL PUSH THROUGH THE MATERIAL.
   - The leveling guide is a small acrylic “L” that fits over the bottom lip of the nozzle and should just touch the material surface.

7. Launch LightBurn on a Lenovo and connect it to the laser using the blue USB cord.

8. Export the file to be cut as a DXF from your CAD software (Fusion 360).

9. Optional but recommended:
   a. Launch Corel on the same Lenovo and import the DXF (Ctrl + I).
   b. If the DXF imports as a group (objects appear under a dropdown in the Objects menu), right-click and select Ungroup (Ctrl + K).
   c. Select all objects and combine them (Ctrl + L).
   d. Ensure nothing is selected, then export as an .AI file (Ctrl + E).

10. Import the DXF or .AI file into LightBurn. If unexpected lines appear, repeat Step 9.

11. Ensure all lines that will have the same operation (cut or engrave) are the same color. Colors can be changed by selecting lines and choosing a color from the bottom toolbar.

12. Set appropriate power and speed settings in LightBurn.
    a. Open the Library window and select your material from the dropdown.
    b. Select the cut thickness.
     c. Select the correct cut layer on the right side and click Assign.
⚠ DO NOT CLICK “LINK.” THIS WILL OVERWRITE THE MATERIAL LIBRARY SETTINGS.

13. Position the laser head over the material.
    -In the bottom right of the Cut window, choose Origin, Current Position, or Absolute Coords.
     a. Origin will start the cut from the last saved origin, not the current head position.
         - This can be updated by moving the laser and pressing the Origin button.
     ⚠ IF RUNNING FROM THE CONTROL PANEL, IT WILL ALWAYS BE IN ORIGIN MODE.

     b. Current Position will start the cut based on the current head position.
        - The 3×3 grid in the Cut window determines where the file will be placed relative to the head position.
        - For example, if the top-left circle is selected, the laser will align the top-right of the file with the head location.
    ⚠ WHEN USING CURRENT POSITION, IF PARTS ARE REMOVED FROM THE CUT FILE, THE LASER WILL CUT BASED ON THE CURRENT FILE SIZE, NOT THE PREVIOUS ONE.

     c. Absolute Coords will cut the file based on its position in LightBurn relative to the machine’s coordinate system.

14. Frame the material using either Bounding Box or Rubber Band frame.
    - Bounding Box creates a rectangle that fully encloses the cut file and traces it. (This is the only option if working from the control panel.)

    - Rubber Band traces the outermost path of the design and is more precise but will not show internal geometry.
⚠ DO NOT HOLD SHIFT WHILE PRESSING FRAME. THIS WILL CAUSE THE LASER TO FIRE AND CUT THE FRAME INSTEAD OF TRACING IT.

15. Begin the cutting process through either LightBurn or the control panel.
    
16. Monitor the cutting process to ensure proper operation
    - Small flames may appear directly under the cutting head.
⚠ NEVER LEAVE THE LASER UNATTENDED WHILE CUTTING. (This has been done before and it caused signifigant damage and signifigant down time)  
⚠ IF A FIRE BEGINS TO GROW, DOES NOT GO OUT AFTER THE CUTTING HEAD HAS MOVED, OR STARTS TO SPREAD:
STOP THE MACHINE IMMEDIATELY USING STOP, PAUSE, OR THE EMERGENCY STOP (E-STOP).
EXTINGUISH THE FIRE USING THE SAND BUCKET LOCATED ON THE GROUND TO THE RIGHT OF THE LASER CUTTER.
FAILURE TO ACT IMMEDIATELY MAY CAUSE SIGNIFICANT DAMAGE TO THE MACHINE AND ITS LENSES.

17. After completion, do not reposition the material. Lightly press on the part to check if it has fully cut through.

18. If the part moves freely, remove it and either begin another cut or shut down the machine (reverse Steps 2–4).

19. If the part does not move freely, repeat the cutting step.


The machine requires daily cleaning of the cutting bed and weekly maintenance of the laser optics. The recommended maintenance schedule includes monthly calibration checks and quarterly deep cleaning procedures.

### 5. Common Troubleshooting

CHECK AFTER EACH STEP., IF THE ISSUE PERSISTS, CONTINUE TO THE NEXT STEP
IF PROBLEMS OCCURRED THAT WERE NOT COVERED IN THIS SECTION, CHECK THE MANUAL LOCATED IN THE TOOLBOX INSIDE OF THE CABINET NEXT TO THE LASER

Bed wont go up and will only go down:
- If the Z height only goes down, check for a red light behind the nozzle, fully lift the nozzle and then let go, then check if the light has disappeared (if it hasn't repeat until it does)

The laser is cutting extremely wide:
- Ensure the z offset is correct by following step 6 of proper use
- Fully lift the nozzle and then let go
- Follow the alignment instructions https://www.youtube.com/watch?v=RbKaCOxGxaA. The tools required are located inside the cabinet next to the laser

Flames are coming off the workpiece:
- Ensure that the powerstrip controling the ventilation is powered on
- Ensure that the air assist is plugged in to the ventilation power strip (the air assist is a small brass pump located on the ground behind the laser)

The laser is not cutting in the expected position:
- Repeat step 13

X/Y slop error (The attempted operation will extend outside of the bed):
- Move, rotate, scale, or segment the cut so that it is completely within the bounds of the bed

The laser cutter is not cutting all the way through:
- If the laser cutter was recently powered on, it will perform worse than after repeated cuts, as the laser needs time to fully warm up
- Ensure the proper cut settings were used (Step 12)





### Control Panel Operation

The Boss laser control panel has specific buttons for operation:
- Z/U buttons to enter the sub menu and then left or right arrow buttons to move the bed up or down
- Arrow buttons to navigate through menus and adjust settings
- Press ESC to exit current menu or cancel operation
- Press ENTER to select options or confirm settings
- Press START/PAUSE to begin or halt the cutting process
- Press ORIGIN to return the laser head to its home position
- Press FRAME to adjust the cutting frame boundaries

### Maintenance Schedule

Regular maintenance procedures include:
- Daily cleaning of the cutting bed
- Weekly cleaning of the laser optics
- Monthly calibration checks
- Quarterly deep cleaning procedures
- Annual comprehensive maintenance by qualified personnel

### Emergency Procedures

In case of emergency:
- Immediately shut down the machine
- Ensure all users are clear of the machine
- Contact a mentor for assistance
- Document the incident for future reference
