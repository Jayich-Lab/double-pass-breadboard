# double-pass-breadboard

This repo tracks our double pass breadboards.  The aim is to realize compact and reliable double pass breadboards.

Different versions of the breadboard are organized in directories labeled by the date that the parts were *initially* ordered - subsequent orders should not change the version.

Each directory should include STEP files for all the necessary parts.  At some point getting drawings in that can be viewed online would be good. Lab useful machining files, such as *.ipt, can certainly be included.

Ideally we get some performance results plotted and include a guide to parts, assembly, etc.  Long term stability, temperature stability, are all to-dos.

<img width="599" alt="cost" src="https://user-images.githubusercontent.com/63123871/231609481-7296a951-1a45-4414-b5d5-492b8e8fb254.png">

# Parts

### Machined parts
Link to location in our drive of the .step files:
https://drive.google.com/open?id=1YvjQak18hdsUjOcQHWJoqq3adjisLcIZ&usp=drive_copy

Hole tapping requirements: the 3.302 mm tapped holes need to be #8-32 screwed, the smaller ones (2.845 mm) will be #4-40 screwed, and the larger ones (5.157 mm diameter) should be 1/4''-20 screwed.

### Newport
* (6x)  ZeroDrift Optical Mount  [ST05-F2H](https://www.newport.com/p/ST05-F2H) (these are interchangeable with polaris half inch low drift mirror mounts that can be ordered from thorlabs)

### Thorlabs
* (1x)  Lens Mount                  [LMR1](https://www.thorlabs.com/thorproduct.cfm?partnumber=LMR1#ad-image-0)
* (1x)  Mounted Standard Iris       [ID8](https://www.thorlabs.com/thorproduct.cfm?partnumber=ID8)
* (2x)  FiberBench Wall Plate       [HCA3](https://www.thorlabs.com/thorproduct.cfm?partnumber=HCA3)
* (2x)  Port Post Mounting Bracket  [HCP](https://www.thorlabs.com/thorproduct.cfm?partnumber=HCP)
* (1x)  AOM Mount                   [KM100PM/M](https://www.thorlabs.com/thorproduct.cfm?partnumber=KM100PM/M)
* (1x)  Plano-Convex Lens           [LA1131-A-ML](https://www.thorlabs.com/thorproduct.cfm?partnumber=LA1131-A-ML)
* (1x)  Dual Rotation Mount         [DLM1](https://www.thorlabs.com/thorproduct.cfm?partnumber=DLM1#ad-image-0)
* (2x)  Achromatic FiberPort        [PAF2A-A10B](https://www.thorlabs.com/thorproduct.cfm?partnumber=PAF2A-A10B)
* (1x)  Polarizing Beam Splitter    [PBS202](https://www.thorlabs.com/thorproduct.cfm?partnumber=PBS202)
* (1x)  Broadband Dielectric Mirror [BB05-E02-10](https://www.thorlabs.com/thorproduct.cfm?partnumber=BB05-E02-10)
* (2x)  Fiber Port Post Mount       [HCP](https://www.thorlabs.com/thorproduct.cfm?partnumber=HCP)


# Next generation improvements to consider

* The lens mount should be able to be translated (similar to the double pass mirror mount).
* Iris holder cannot be flipped 180 degrees because it is too wide; in the current position the iris adjustment faces into the board and is difficult to reach with my fingers when the aperture is open  
* Some of the edges could be trimmed to make the board even smaller.
* Maybe use channels for the screw holes in the mirror mounts so they can be translated continuously; although, this may complicate the design with little benefit.  
* Check operation of the collars on mirror mounts - tightening them sometimes messes with alignment  
* Fiber holders should be the same model
