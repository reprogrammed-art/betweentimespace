# Between Time and Space
The documentation of the artwork Between time and space, Martin Frohlich, 2015
Version 1.0  2015.03.16
CC-BY Martin Fröhlich
http://www.maybites.ch/works/betweentimeandspace/



**Bill of Materials**

- 1 x	wooden board of approx. 900 x 900 x 18 mm
- 2 x 	square alluminium bar. l = 1m / 20 x 20 mm, 2mm wall strength
- 1 x 	sheet plexiglas of  approx. 900 x 600 x 6 mm
- 1 x 	sheet plexiglas of  approx. 900 x 600 x 4 mm
- 1 x 	sheet plexiglas of  approx. 400 x 400 x 1 mm
- 50 x 	Ballbearings 9 / 4 / 4 mm
- 2 x	Ballbearings 42 / 20 / 12 mm
- 1 x	Brass rod  l= 1m /  d = 4 mm (pairs with the 9/4/4 ballbearings)
- 2 x 	Copper rod l = 1m / d = 1.45mm
- 2 x 	Copper rod l = 1m /  d = 1.55m
- 1 x 	Acryllic two-component glue
- 1 x	instant adhesive superglue (i.e. Loctite 401)
- 1 x 	elastic l = 2m / d = 3mm. 
- 8 x 	rivets (see shape and dimension inside blender file)
- 1 x	DC electromotor with approx. 120 - 240 rpm.

**What to take care of when choosing the materials:**

the plexiglas I used was not in the thickness specified. The 6mm thick one was between 5.9 and 6.3mm (which was not so crucial), but the 4mm thick one was between 3.5 and 4.1 mm, which caused some problems because the pieces that needed to be stuck together where not tight enough. Or sometimes they didn’t fit because to thick. Or something stuck out because to thin. So make sure the thickness of the plexi is as close to its specified thickness. Don’t measure just at one corner, measure all corners.

The small ball bearings and the brass rod have to fit each other. Make sure they do lie within the right tolerances. If in doubt, ask an expert. Spend some time on this, because if the pairing is wrong, you will spend hours to fix this. (using a drill and sandpaper to sand down the diameter). Spend some more money to get high quality bearings. If you don’t find the same bearings as specified, don’t worry, just make sure this pairing is right. You can correct all the other things inside blender and exporting the objects again.

The 1.45mm copper rod is used to lock the brass-shaft against rotation. It pairs well with a 1.5mm drill bit (see more about this later)

The 1.55mm copper rod is used to stick pieces together before they are glued, to make sure they stick to the right position.

Both diameters are a bit arbitrary, and if you dont find them in your hardware shop, you can choose different ones, but make sure you pair the one for the lock against rotation with an available drill. And make changes inside blender accordingly.

The elastic has to be as flexible as possible and should not take much force to pull. It should be able to expand to at least twice its relaxed length, more is even better.

The rivet has the task to hold the elastic and simultaneously as a guide bearing for the seamless  elastic ring that encompassing all four rivets.

The superglue is used to stitch together the elastic to the seamless ring. Loctite  Super Attak or Loctite 401 should do the job.

Before cutting the Pieces

The current files (and the blender design) are dimensioned according to the tolerances of the lasercutter I had at my disposal (Epilog). Its laser diameter was close to 0.15 mm. But your lasercutter might have different characteristics, so before you cut all the pieces, make some tests to see if the current files fit accordingly.

Pairs to test  (you don’t need to print out the complete big pieces, just the parts that matter): 

*WheelCage – WheelCageDistancer (tight)
*WheelCage – small Bearings (strong pressing force needed)
*WheelCage – 1.55 mm copper rod (tight)
*DriverBase – small Bearings (strong pressing force needed)
*DriverBase – big Bearing (strong pressing force needed)
*DriverBase – WheelCageDistancer (tight)

Several 4mm gears need to have the 4mm brass rod as a shaft. This has to be super tight for ALL of them (see blender): 
*example for 4mm: Gear_Spur_Lever_Driver
*example for 6mm: Lever

if the above requirements are not met, you either

	1.	adjust the diameter of the holes inside blender and export the files again. You need the svg exporter to do this: http://wiki.blender.org/index.php/Extensions:2.6/Py/Scripts/Import-Export/Inkscape_SVG_Exporter
	2.	adjust the current files inside Inkscape or Illustrator or any other vector program. Make sure the scaling doesn’t play a prank on you (as it did on me).


**Preparations**
After cutting the Pieces

Unfortunately right after cutting the pieces comes the hard part. Because the elastics put significant force onto the whole drive, there are some momentums that have to be checked with rotation locks at certain parts. All the following pieces need to have a 1.5mm hole drilled into them (see in detail blender file):

Gear_Spur_Lever_Multiplier <->  Lever Pair

Shaft is 3.7cm long, the holes are 7mm from each end.
Gear_Spur_Head <-> Head Pair
Shaft is 1.9mm long, gear-hole is 2mm from end, head-hole is 3mm from end.

However, this has to be done so precisely, that I had a more than 50% waste. The newly drilled hole has to go perfectly centric through the hole for the shaft, otherwise you will not be able to put the rotation lock-pin through the shaft.

And, even more tricky, the shafts themselves need each two 1.5mm hole drilled precisely centric and perpendicular to the rod and parallel to each other. For this I had to create a boring template because the 1.5mm drill is very flexible, and drilling a round rod like this is very tricky. If you don’t have mechanical expertise you should consider asking a mechanic to do this for you. The more precise you work here, the less problems you will have during the assembly.

**Board**

Before you can start with the final assembly you need to prepare the Board on which the whole piece is assembled, with the right holes at the right place. There is no plan in existence for this, and  blender will give the right coordinates, at least for the holes of the attachment of the two big drives. The MirrorBase has a design that allows adjustment of the distance to the DriverBase, so slight imprecisions can be corrected. But drilling the holes for the TransmissionCage I suggest a different approach. First assemble the MirrorBase with its Gear and the DriverBase with its Gear and attach it to the board with the proper screws and tight things up as they would be at the final assembly. Then roughly place the TransmissionCage on the board where it should be, and stick the assembled Gear_Spur_130 with shaft into its assign hole of the TransmissionCage. This way you can see how far away the TransmissionCage needs to be so the Gear_Spur_20 pairs up with the Gear_Spur_160 in a fitting way. Now you can drill the holes for the TransmissionCageHolder and use the holes of the TransmissionCage as a guide. Once this is done remove the Gear_Spur_130 and drill this hole as well.  Now you can assemble the Transmission and place the motor in a similar way. I dont give here specific instructions on how to do this, the blender file gives a suggestion on how big a hole you need and how you could attach the motor to the board and its gear. But since I don’t know the form factor of you motor, I will have to leave this problem to you and you ingenuity. 
Once all the holes are done and the motor problem is solved you can disassemble everything. Now you can attach the two square aluminum bars at the back, one near the top, one near the bottom. This gives some space in the back for the motor. If 20mm is not enough because your motor needs more space then choose the dimensions accordingly.
Once all the work on the board is done, it can be finalized with paint or any other fancy means.
Assembly

The explosion drawings used in this document were done before I finalized the object, so they differ in some details to the blender file and the final piece. I will add explanations where it is needed to point out some differences or best practices.
Transmission

Check the length of the TransmissionCageHolder and the Shaft_Spur_20mm inside blender. In my solution I used a LeverMultiplyer_Distance_4mm to fix the TransmissionCage to the CageHolder. (this also needs to be is a very tight fit – see above). The little hole inside Gear_Spur_20, TransmissionGearDistancer and Gear_Spur_130 is for a 1.55 copper rod as a rotation lock.

**DriverBase**
The DriverBase looks now a bit different. At the end I didnt use the MasterBearingDistancer, but made sure the 3 MasterBearing_CentralRod are super tight inside the ball bearing and the bearing has some space to the DriverBase. There is now a new piece called MasterBearing_CentralTopRod. Check blender for more details. The MasterBearing_CentralRod is glued to the DriverBase with superglue. Be careful though: The new design has also a different Main_Shaft_TorqueStop (see next step) that goes into the DriverBase. Everything needs to be super tight, so it can disassembled if needed, but has no play what's however.
The DriverBase is actually only attached to the board at the end of the complete assembly of the drive.

**MasterCog**
The sequence of assembly is actually a bit different than depicted here and the last picture. I put the BallBearing 42/20/12 first into the Gear_Spur_160 with some superglue. Because of the superglue this has to be done very quickly, and it has to be done very precisely otherwise the Gear is not level to the board. Also press the BallBearing_9/4/4 into the Gear_Spur_160 before assembling it with the DriverBase. (see blender for correct positioning)
The Main_Shaft_TorqueStop and Gear_Elliptical_42 are glued together before assembly. The new piece MasterBearing_CentralTopRod can be glued to this combo, too. (See blender for details).
Be careful: don’t mix  Gear_Spur_160_M2_Driver with Gear_Spur_160_M2_Mirror, they are not the same!!!
TimeGear

The little holes in the gears are for the 1.55m copper rod as a rotation lock. Make sure your gears are placed as show here, so the elliptical gears align properly. The Shaft_4.6cm is now 3.7cm and there are 1.5mm holes in the shaft and the Gear_Spur_Lever_Multiplier. (see under Preparations)


**TimerGear Completed**
Before you can get to the next step, you need to assemble the cogs accordingly. It is of utmost importance that the cogs don’t jump a teeth, otherwise the elliptic gears get stuck and the timing would be off.
WheelCage

First glue the WheelCage_Distancer to the Gear_Spur_160. The WheelCage_Distancer have actually a new design so the WheelCage can now be screwd to them. Before you can do this, you need to drill to countersunk the dedicated holes in the WheelCage. Use M3/12mm countersunk-head screws with bolts and make sure the head of the screw is not sticking out. Otherwise a collisions can happen. The same actually applies to the WheelCage_Distancers. Make sure they dont stick out the WheelCage. If they do (in my case the plexi of the WheelCage was not thick enough) shorten them before you assemble the pieces. The Head_Driver_DistanceRing is obsolete and the Gear_Spur_Head_Driver will be attached (glued – use the copper rods to place it correctly!!) directly to the WheelCage. Here it shows how well the shafts and the bearings are paired (See Bill of Materials).
Lever

Make sure you align the pieces exactly as shown here. Shaft_16mm is actually 19mm long (See Preparations). I suggest to assemble the complete Lever before attaching it to the Drive. Do not forget to install the rotation locks. Use clear sticky tape or wood glue to keep them inside. The slits in the pieces that need the  rotation-locks are there to remove the lock-pins. So make sure you dont make the lock-pins to long, so you can use a pointy device to take them out again (rest assured – you will have to). The Head_Plate has now two holes for two 1.55mm pins that allows to stick it into the Head. The rivet should only be pushed with force into the Head_Plate. This allows easy attachment/replacement of the elastics.
Lever Completed


**MirrorBase**
The Design of the MirrorBase has changed with features to attach it to the Board with M6 hexagonal head screws. There is also a M4 hexagonal head screw to attach the MirrorBase to the MirrorBase_AngleBracket which allows for shifts to set the correct distance for the two big wheels once they are assembled. Follow the same assembly instructions as with the DriverBase.

**MirrorCog Completed**
Repeat the assembly with the MirrorDrive. However you have to look at it from the other side. Make sure the Gear_Elliptical_42_0.08_Slave looks the other way. Check first blender to get properly started – even I had to reassemble the MirrorDrive twice.

**Completion**
The rivets and Head_Plates are not assembled yet. The Head_Plates have the 1.55 mm pins glued into them so they can be stuck onto the Heads.
I used needle and a very tough thread to pull the elastics through the rivets first. The length for the four connecting elastics is measured on the piece at the point where the two opposing Heads are closest to each other. The elastic should be just barely pulled at this point to reduce the forces as much as possible. Once all four elastics are riveted, they can be pushed into the Head_Plates, but only so deep that the two elastic circular bands can slide between rivet-head and Head_Plate. Then rotate the wheels  45 degrees from the assembly position. Now measure the length for the circular bands. This position is the shortest length. Again make sure to set the length of the bands so that they just barely pull. Use superglue to stick the two ends together.
Now you can assemble all the elastics. If the holes inside the Head were dimensioned right, the Head_Plates should not be pulled out during operation. If they do, just slightly bend the 1.55mm pins. You don’t wanna glue them, because then you will be in trouble if you need to disassemble the piece again.

Assuming you found a solution for attaching your motor the piece is ready for a run. I first slowly run it by hand to check of there are no collisions and other mechanical problems, because once the elastics are installed, they apply quite a pull to the whole structure and it behaves differently than without. 

Once you are confident that it should run smoothly, take a deep breath and plug it in.

If you can breath again and see what I saw for the first time on the 28th of February 2015, then you have to tell me about it. Please. :-)


