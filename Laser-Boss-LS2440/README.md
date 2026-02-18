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
1. Ensure the bed is empty and the laser nozzle with not hit anything if it moves completly to the far right
2. turn the key located above the control panel to turn on the laser (it will automatically home so be ready for it to move)
3. Flip the switch located on the front of the white box on the floor to the right of the laser to turn on the cooler
4. Flip the switch on the power switch mounted to the wall on the left side of the laser to turn on the air assist and exaust (note this can be turned on later to avoid noise but MUST BE TURNED ON BEFORE CUTTING)
5. Load the material to be cut onto the cutting bed
   - if the material is to small for the slats a mesh bed is located to the left of the laser which can be put ontop.
   - If the material is too big to fit in the laser the red pannels surrounding the laser can be either opened or removed (The pannels on the back and sides are opened through a latch in the middle (the latch should be closed with the door open to allow material to lay flat) the pannel in the front can be removed by pulling the latches located inside of the hollow bar on either side)
6. Adjust the Z-height using the control panel for optimal cutting depth (This can be done through either using the auto focus or the leveling guide)
   - THE NOZZLE MUST MOVE FREELY UP AND DOWN BEFORE USING THE AUTOFOCUS
   - The leveling guide is a small acrylic L that fits over the bottom lip on the nozzle and should touch the material
7. launch lightburn on a lenovo and connect it to the laser through the blue usb cord
8. Export the file you want to cut as a DXF by creating a drawing in the CAD software (Fusion 360)
9. Optional but recomended:
    a. Lauch Corel on the same lenovo and import the DXF into it (CTRL + I)
    b. If the DXF imports as a group (the lines and curves are under a dropdown menu in the objects menu) ungroup them by right clicking and pressing ungroup from the droupdown menu (Might be CTRL + K)
    c. select all objects on the screen and combine them (CTRL + L)
    d. Make sure nothing is selected and export the file (CTRL + E) as a .AI
10. Import the DXF or .AI file to Lightburn (if unexpected lines apear follow the previous step)
11. Ensure all lines that will have the same operation performed on them (Cut/Engrave) arae the same color (the color can be changed by slecting lines and choosing a color from the botom task bar)
12. Set appropriate power and speed settings in Lightburn
   - Open the library window in lightburn and select the drop down for your material
   - Select the cut thickness from the drop down
   - on the right side select the cut layer and then click assign (DO NOT CLICK LINK THAT WILL UPDATE THE LIBRARY WITH YOUR SETTINGS)
13. Position the laser head over the material
   - On the bottom right of the cut window there is a drop down where you can choose Origin, current position, or absolute coords
     a. Origin will always start the cut from the last saved origin not the current position (this can be updated by moving the laser and pressing the origin button) (IF RUNNING FROM CONTROL PANNEL IT WILL ALWAYS BE IN THIS MODE)
     b. current position will start the cut based on the current position of the head
        - on the bottom right of the cut window there is a 3 x 3 grid of circles which determine where the cut file will be placed in relation to its current position (ie if the top left circle is selected the laser will place the cut file so that the top right of whatever is cutting lines up with the laser) (NOTE WHEN USING CURRENT POSITION IF PARTS ARE REMOVED FROM THE CUTFILE THE LASER WILL CUT BASED ON THE CURRENT SIZE OF THE CUT FILE NOT THE PREVIOUS ONE)
     C.  Absolute coords will cut file based on the positioning in light burn and both the origin and current position of the head
14. Frame the material with either the bouding box or rubberband fram
    - The bounding box frame will create a rectangle that completly fits the cut file and trace that on the laser (this is the only option if working from the control panel)
    - The rubber band frame will trace a path that could be found by putting a rubber band around the part (This will provide a more accurate frame but will still not show inside geometry)
    - DO NOT HOLD SHIFT WHILE PRESSING THE FRAME BUTTON THIS WILL CAUSE THE LASER TO TURN ON AND CUT THE FRAME INSTEAD OF TRACING IT
14. Begin the cutting process through eithe lightburn or the control pannel
15. Monitor the cutting process to ensure proper operation
    - Small fires may start directly under the head
    - IF FIRES GROW, DO NOT STOP AFTER THE CUTTING HEAD HAS MOVED, OR SPREAD STOP IMMEDIETLY(press the stop, pause, or estop button) AND EXTINGUISH USING THE SAND BUCKED ON THE GROUND TO THE RIGHT OF THE LASER CUTTER FAILURE TO DO SO WILL CAUSE SIGNIFIGANT DAMAGE TO THE MACHINE AND ITS LENSES
16. After completion, do not move the part  and lightly touch if to see if it moves
17. if the part moves remove and either start another cut or turn it off (opposite of steps 2-4)
18. if the part does not move return to step 14


The machine requires daily cleaning of the cutting bed and weekly maintenance of the laser optics. The recommended maintenance schedule includes monthly calibration checks and quarterly deep cleaning procedures.

### 5. Common Troubleshooting

Common issues users encounter with the Boss laser include:
- Inaccurate cuts due to improper Z-height adjustment
- Burn marks or charring on cut materials
- Error messages on the control panel
- Laser head not moving properly
- Uneven cutting edges
- If flames are coming off the workpiece, make sure the air assist is open all the way

For Z-height adjustment problems:
- The autofocus feature can be problematic on softer materials (cardboard) and the z height gauge should be used instead
- Always use the control panel method for precise Z-height adjustment
- If the Z height only goes down, check for a red light behind the nozzle, fully lift the nozzle and then let go, then check if the light has dissapeared (if it hasnt repat until it does)
- Use the Z/U buttons to make precise adjustments
- Use the ORIGIN button to reset the laser head position if needed

For other common problems:
- Check that the material is properly secured on the cutting bed
- Verify that the laser power and speed settings are appropriate for the material
- Ensure the laser lens is clean and free of debris
- If issues persist, contact a mentor for assistance

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
