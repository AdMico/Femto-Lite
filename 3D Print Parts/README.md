# LipidWells v1.0.0 (Updated 01APR26 APM)

**Written by:** Adam Micolich

## Contents of the *CNC Parts* folder

This folder has two sub-folders: *MUXBox* and *Stage Parts*

## Contents of the *MUXBox* folder

This folder has CNC-ready STEP files for all the various panels and structures of the multiplexer box (aka MUXBox). The various files are as follows:

`MUXBox_Back_V1-Body.step`: This makes the rear wall of the MUXBox, which supports the four bulkhead BNC connectors and the rear 2 x 9V battery housing.

`MUXBox_Bottom_V1-Body.step`: This makes the baseplate of the MUXBox, with screwpoints for mounting the Mux Board PCB.

`MUXBox_Front_V1-Body.step`: This makes the front wall of the MUXBox, which supports the front 2 x 9V battery housing.

`MUXBox_Left_V1-Body.step`: This makes the left wall of the MUXBox, which supports the sidepanel PCB, which acts as a feedthrough for the two 30-pin and one 40-pin ribbon cables.

`MUXBox_PiHolder_V1-Body.step`: This makes a 'cage' for holding the Raspberry Pi down onto the TopLeft panel of the MUXBox, it is designed to fit the aluminium heatsink specified in the parts list in the *PCBs & Schematics* folder.

`MUXBox_Right_V1-Body.step`: This makes the right wall of the MUXBox, which is a clean panel.

`MUXBox_TopLeft_V2-Body.step`: This makes the top-left lid panel of the MUXBox, which is designed to support the Raspberry pi, which is held in place by the PiHolder mentioned above.

`MUXBox_TopRight_V1-Body.step`: This makes the top-right lid panel of the MUXBox, which supports the two DPDT toggle switches, four SPST momentary switches and four panel-mount LEDs (2 x red, 2 x green) specified in theparts list in the *PCBs & Schematics* folder.

The panels are designed to be machined in aluminium, which is then bead-blasted and anodised, and can be readily done via a company such as PCBway or JLCPCB. I tend to hand-tap the threaded holes myself, both to reduce the CNC cost and ensure the threads are done well.

Any holes in these panels will either be drilled to 3mm diameter, and be clearance holes for an M3 bolt, or be drilled to 2.5mm diameter, ready to be tapped to M3 as a threaded hole for an M3 bolt. It is easy to check which is which using an M3 bolt. ;)

A photograph of a fully assembled MUXBox can be found in the *PCBs & Schematics* folder.

## Contents of the *Stage Parts* folder

This folder has CNC-ready STEP files for all the various components for mounting one of our OECT-coverslips onto a fluorescence microscope. The components are designed for one of two microscope stages. The first is the Marzhauser Wetzlar SCAN IM 120 x 88 stage. The second is the Mad City Labs uS-2308 stage. We use the latter on our current microscope configuration. The various files are as follows:

`Stage_Assy_1.jpeg`: Photograph of the stage assembly with one of the two stages, the Baseplate and the Pinplate shown. The various PCBs and spring-pins are assembled onto the Pinplate.

`Stage_Assy_2.jpeg`: Photograph above with a pair of the Mount Supports in place, which are designed to assist with optimum contact of all 54 spring-pins onto a coverslip.

`Stage_Assy_3.jpeg`: Photograph above with the addition of the five components of the top cover assembled. The two ribbon cables feed through the slots in the cover provided.

`Marzhauser_Stage_Gen4_V1-Body.step`: CNC-ready file for an adaptor plate to mount our Baseplate for supporting the rest of the assembly on a Marzhauser Wetzlar SCAN IM 120 x 80 microscope stage.

`MCL_Stage_Gen4_V1-Body.step`: CNC-ready file for an adaptor plate to mount our Baseplate for supporting the rest of the assembly on a Mad City Labs uS-2308 microscope stage.

`Baseplate_Gen4_V1-Body.step`: CNC-ready file for the Baseplate, which fits into either the Marzhauser stage plate or the Mad City Labs stage plate, and features the cut-out for the coverslip to be positioned into. The four vertical posts are for bolting down the Pinplate assembly.

`Pinplate_Gen4_V1-Body.step`: CNC-ready file for the Pinplate, which holds the various PCBs for mounting the Harwin spring-pins that interface to the 54 device contacts on the coverslip.

`Mount_Support_Gen4_V1a-Body.step`: CNC-ready file for the two Mount Supports, which enable the height of the Pinplate to be set for optimum contact of the spring-pins to the coverslip.

`Coverwall_Gen4_V1-Body.step`: CNC-ready file for the wall of the cover assembly, which bolts onto the Baseplate.

`CoverTopside_Gen4_V1-Body.step`: CNC-ready file for the two edge pieces of the top-plate of the cover assembly, which bolt onto the cover wall.

`CoverTopmid_Gen4_V1-Body.step`: CNC-ready file for the centre piece of the top-plate of the cover assembly, which bolts onto the cover wall.

`CoverTopcent_Gen4_V1-Body`: CNC-ready file for the hole cover for the centre piece listed above. This enables a user to 'peek inside' the cover without needing to disassemble it.

The panels are designed to be machined in aluminium, which is then bead-blasted and anodised (ideally black), and can be readily done via a company such as PCBway or JLCPCB. I tend to hand-tap the threaded holes myself, both to reduce the CNC cost and ensure the threads are done well.

Any holes in these panels will either be drilled to 3mm diameter, and be clearance holes for an M3 bolt, or be drilled to 2.5mm diameter, ready to be tapped to M3 as a threaded hole for an M3 bolt. It is easy to check which is which using an M3 bolt. ;) The one exception is the Pinplate, where there are a set of 1.6mm diameter holes, ready to be tapped to M2, as threaded holes for holding the PCBs in place on this part of the assembly. Use considerable caution in tapping the M2 holes, an M2 tap is very easily broken, especially in deeper holes, whereupon it is basically impossible to get out (trivia: I once had to, from an irreplaceable piece of gold-plated copper for a diode-laser assembly, and we ultimately had to 'cook' it out using a modified arc welding assembly -- the job took 2 days and an uncountable number of swear words before success was finally achieved).

A final note regarding the mount supports. They are intended to be put in place as supports and removed once the pinplate is correctly in place. As such, screw down until the pinplate just makes contact with both mount supports (they should just be unable to be slided out), then loosen each screw just enough for them to be slided with some mild friction, and the height should be correct.
