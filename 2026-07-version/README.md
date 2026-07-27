# README

This version of the double pass breadboard was first ordered in July 2026. The design builds off the [2024-04-version](https://github.com/Jayich-Lab/double-pass-breadboard/tree/updated-README-for-2026-07-version/2024-04-version), with two additional mirrors and a fiberport for frequency unshifted light pickoff (this is optional when setting up the board). It also features a new AOM mounting system and several other changes:
* The AOM is now attached to a model-specific L-bracket that screws into a kinematic mount which enables fine adjustment of the AOM position. The kinematic mount is attached to an elongated version of the [2024-04-version](https://github.com/Jayich-Lab/double-pass-breadboard/tree/updated-README-for-2026-07-version/2024-04-version) rotation mount, which provides a coarse degree of freedom during initial alignment. This rotation mount is now secured to the board with two screws for improved stability.
* Reduced the footprint of the polarizing beam splitter mount.
* Increased the number of mirror mount holes to nine for most mirrors.
* Redesigned the lens mount to add a translational degree of freedom perpendicular to the beam axis.
* Added more holes to the breadboard base to provide a coarse degree of freedom over both the lens and mirror positions perpendicular to the beam axis.
* Increased the board height by 1.50 mm to ensure all threaded holes have more than three threads for screw engagement.
* Eliminated the mirror between input fiber port and polarizing beam splitter.
* Added a half waveplate before the frequency shifted output fiber port.
* Decreased the overall footprint (possible because of switch to vertical drive mirror mounts).
* Fixed an issue with mounting hole positions so that all three mounting holes can be used simultaneously to mount the board to optics table.
* In order to make changes listed above, the positions of several components were changed from the previous version.
* Switched to using [Thorlabs PAF2 series collimator](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=2940) model with smallest available focal length (PAF2A-A4x) because we have found that reducing beam waist improves efficiency (because AOM aperture diameter is on the order of beam waist).
# Parts

<img src="2026-07_DP_breadboard_schematic.jpg" width="700">

### Parts to be machined
[CAD and drawing files (.step, .ipt, .pdf)](https://drive.google.com/drive/folders/13lI2C9mWSC0sEyA27Yh_0JeaD-pgw3mP)

* 1x breadboard_base
* 3x waveplate_mount
* 1x PBS_mount
* 1x iris_mount
* 1x lens_mount
* 1x mirror_mount
* 1x company_AOMsize_kinmount (AOM to kinematic mount bracket - there are different parts depending on the AOM used)
* 1x company_AOMsize_base (rotating kinematic mount base plate - there are different parts depending on the AOM used)

This board could be adapted for AOM models beyond the three we use, but the last two parts in the above list would need to be redesigned.

### Mirror mount
* 7x [Thorlabs POLARIS-K05VS2](https://www.thorlabs.com/item/POLARIS-K05VS2) (5x if board setup without unshifted light pickoff)

 The three mirror positions near the exterior edge of the board are compatible with other horizontal-drive 1/2" mirror mounts. The four sets of mount holes that sit away from the edge are designed only for vertical-drive 1/2" mirror mounts. Using horizontal drive mounts for these would make alignment extremely difficult because of limited screw access.
 
### Wuhan Union Optic Inc.
* 2x Quarter waveplates
* 2x Half waveplate
* 1x Polarizing Beam Splitter (PBS)

We get our waveplates and PBS from [Union Optic](https://www.u-optic.com/). If the waveplates are not in the standard [Union Optic catalog](https://www.u-optic.com/product) we order custom waveplates; this is often the case.

### Thorlabs
* 1x [LMR1 Lens Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=LMR1#ad-image-0)
* 1x [ID8 Mounted Standard Iris](https://www.thorlabs.com/thorproduct.cfm?partnumber=ID8)
* 3x [PAF2A-A4B Achromatic FiberPort](https://www.thorlabs.com/item/PAF2-A4B) (2x if board setup without unshifted light pickoff)
* 3x [HCA3 FiberBench Wall Plate](https://www.thorlabs.com/thorproduct.cfm?partnumber=HCA3) (2x if board setup without unshifted light pickoff)
* 1x [LA1131-B-ML Plano-Convex Lens](https://www.thorlabs.com/thorproduct.cfm?partnumber=LA1131-B-ML)
* 1x [RSP1 Single Rotation Mount](https://www.thorlabs.com/item/RSP1)
* 1x [DLM1 Dual Rotation Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=DLM1#ad-image-0)
* 1x [BB05-E02-10 Broadband Dielectric Mirror](https://www.thorlabs.com/thorproduct.cfm?partnumber=BB05-E02-10)
* 1x [LM1-B Rotation Mount](https://www.thorlabs.com/thorproduct.cfm?partnumber=LM1-B)
* 1x [LM1-A Rotating Inner Carriage](https://www.thorlabs.com/thorproduct.cfm?partnumber=LM1-A)

Note: the optics above are an example that can be used for 728nm light. 

# Future improvements

* The addition of beam shaping optics before the AOM can improve diffraction efficiency.
