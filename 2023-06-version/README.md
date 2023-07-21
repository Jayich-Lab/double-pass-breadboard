# README

This version of the double pass breadboard was first ordered in June, 2023. This is similar to the 2023-03-version but with a smaller base and unnecessary holes have been removed. The waveplate mounts have been extended to move the moutning screw further away from the waveplate housing. The fiber ports are mounted directly to the base. A machined mounting plate for the lens has been added.

# Parts

### Parts to be machined
[STEP files](https://drive.google.com/drive/folders/1tglj8InTGoLq4X3He1ftFIY83VYrIk3X?usp=drive_link) for the parts to be machined.

* 2x waveplate_mount
* 1x PBS_mount
* 1x mirror_slide
* 1x iris_mount
* 1x lens_mount
* 1x breadboard_base

### Newport
* 6x [ST05-F2H ZeroDrift Optical Mount](https://www.newport.com/p/ST05-F2H)

### Wuhan Union Optic Inc
* 2x Quarter waveplates
* 1x Half waveplate 
* 1x Polarizing Beam Splitter (PBS)

We get our waveplates and PBS from [Union Optic](https://www.u-optic.com/index/siteid/2.html). If the waveplates are not in the standard [Union Optic catalog](https://www.u-optic.com/index/siteid/2.html) we order custom waveplates, this is often the case.

### Thorlabs
* 1x [LMR1 Lens Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=LMR1#ad-image-0)
* 1x [ID8 Mounted Standard Iris](https://www.thorlabs.com/thorproduct.cfm?partnumber=ID8)
* 2x [HCA3 FiberBench Wall Plate](https://www.thorlabs.com/thorproduct.cfm?partnumber=HCA3)
* 1x [KM100PM/M AOM Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=KM100PM/M)
* 1x [LA1131-B-ML Plano-Convex Lens](https://www.thorlabs.com/thorproduct.cfm?partnumber=LA1131-B-ML)
* 1x [DLM1 Dual Rotation Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=DLM1#ad-image-0)
* 2x [PAF2A-A10B Achromatic FiberPort](https://www.thorlabs.com/thorproduct.cfm?partnumber=PAF2A-A10B)
* 1x [BB05-E02-10 Broadband Dielectric Mirror](https://www.thorlabs.com/thorproduct.cfm?partnumber=BB05-E02-10)
* 1x [LM1-B Rotation Mount]((https://www.thorlabs.com/thorproduct.cfm?partnumber=LM1-B))
* 1x [LM1-A Rotating Inner Carriage](https://www.thorlabs.com/thorproduct.cfm?partnumber=LM1-A)

# Future improvements

* The fiber port mounting holes are too small and a washer needs to be used between the port and breadboard base. Make these holes deeper and give the coutner-bore a slightly larger radius to account for machining tolerances
* Model the lens mount after the waveplate mounts, particularly the counterbored screw hole. Make this a translation stage (like the double-pass mirror) for aligning the distance between the lens and AOM.
* Fix the AOM position (eliminate the kinematic mount)
* The iris listed above comes with a glued in screw which can be difficult to remove and is too short to use with the aluminum mount
* Make more space around the iris holder so it does not get as close to the wavplate housing, possibly redesign how the iris is mounted
