# double-pass-breadboard

This repo tracks our double pass breadboards.  The goal is to realize stable, modular, and compact double pass AOM systems for controlling the frequency and amplitude of laser light.  This project was directly inspired by work in [Ike Chuang's group](http://web.mit.edu/~cua/www/quanta/).

Different versions of the breadboard are organized in directories labeled by the date (YY-MM) when the parts were *initially* ordered.  Each directory includes a README with a link to the corresponding STEP files (GitHub doesn't support the STEP file format) for the parts to be machined.


Assembled 2023-03 version:  
 <image img src="./2023-03-version/2023-03-assembled.jpg" width="600"></image>


# To-dos
* Measure performance - long-term stability, temperature stability, 
* Annotate a picture of a fully assembled breadboard, including laser paths to help clarify the instructions below.  
* Diagram of the double pass setup.


# Assembly notes

* Clean the machined parts before assembling.  
* Center the laser light on the mirrors, waveplates, and PBS.  
* Know the desired target center frequency and desired bandwidth.  

### Polarizing Beam Splitter Handling
We use [Devcon 5 Minute Epoxy](https://itwperformancepolymers.com/products/devcon-5-minute-epoxy/) to secure polarizing beam splitter (PBS) cubes to their mounts. 
- Note: use only a little dab of epoxy for a single corner and avoid the joint between the two halves of the cube. If epoxy contacts this joint, it will seep in over time, eventually ruining the PBS.

### Waveplates
After the input fiber port is a quarter waveplate and a half waveplate. The waveplate after the AOM is a quarter waveplate.

### Maximizing Double Pass Efficiency
* Place the input fiber port, adjust two mirrors until the beam is horizontal. The beam should not be diverging anywhere throughout the breadboard, so it is important to use a beam profiler to measure the beam far away (~80cm) from the fiber port and use Zθ1, Zθ2, and Zθ3 on the input port to minimize beam divergence. This step is important to get decent AOM diffraction efficiency reasonable output fiber coupling.
* Place the half wave plate and PBS in the beam path.
* Place the AOM. Adjust the height of the incoming beam so the beam passes through the aperture's center. Keep the beam horizontal when adjusting the beam height. If the beam is too high or too low the beam will be clipped or not symmetric on the beam profiler.
* Place an iris after the AOM to select the desired diffraction order. Adjust the AOM's angle to maximize diffraction efficiency at the desired AOM center drive frequency. 
Check the single pass bandwidth by changing the AOM driving frequency. Adjust the AOM to make sure that efficiency is high enough for the frequency of interest. Also make sure the first order beam is not clipped by the iris. Measure the single pass bandwidth (and plot).
* Place an plano-convex lens, e.g. f = 50 mm, after the AOM with convex side facing the AOM. Place the lens approximately a focal length away from the AOM. Adjust the height of the lens so the beam is centered on the lens. Adjust the position of the plano-convex lens so the spacing between the first and zeroth order beams do not chang after the lens. This step is crucial for getting a good double pass efficiency.
After setting the distance between the AOM and plano-convex lens, place the lens so the first order beam passes through the lens center. There are some references saying it would be better to let the zeroth order beam pass through center of the lens, but I (Mingyu) found aligning it with the first order beam actually improves the bandwidth.
* Place the beam profiler about a focal length away from the lens, and try to find the spot where the beam width is the smallest.
* Put a flat mirror at the smallest beam width position, and adjust the mirror so it reflects the light back into the AOM following the same path. Put a quarter wave plate in front of the mirror.
* Keep the first order beam selected using the iris. Adjust the quarter wave plate and the flat mirror until the light reflected back from the PBS is maximized.
* Check the double pass efficiency before fiber coupling. Check the bandwidth. It should be smaller, but comparable to the single pass bandwidth recorded in step 6.
* If the bandwidth is significantly smaller for the double pass, then adjust the distance between the AOM and the lens to improve the bandwidth.
* Couple the light into a fiber using two mirrors. Check the after fiber coupling efficiency.

### Fiber coupling with Thorlabs collimator
* First connect a multi-mode(MM) fiber to the ouput port for initial coupling. Use reverse fiber coupling method to get a rough alignment between output fiber and the laser. The reverse fiber coupling is accomplished by inputing another beam with a visual fault locator from the other end of the output fiber and match the locator beam path to the output beam path.
* Turn Zθ1 adjuster clockwise to maximize the output, then continue to turn slightly beyond maximum (to about 95% of your local maximum). If turning an adjuster clockwise decreases output, skip that adjuster for that round of adjustments. Repeat for Zθ2, and then Zθ3. For the rest of the colimation process keep this order of operation (Zθ1-->Zθ2-->Zθ3). The maximum seen in passing will continue to increase until lens-to-fiber spacing is optimized (spot size is minimized). This strategy has the effect of translating the beam in a triangle of decreasing width with each set of adjustments. The beam's path is shown below with the point of view of the fiber that is being coupled into.
* ![image](https://github.com/Jayich-Lab/double-pass-breadboard/assets/101778987/13e20d5a-d1d1-453d-8352-f6e63863dda7)
* Once the local maxima values begin to decrease, reverse the direction, and turn each adjuster to maximize the output, and not beyond.
* If coupling into a single-mode(SM) fiber, exchange the MM fiber with a SM fiber. The intensity measured by the power meter will likely drop significantly. Repeat Steps 3 and 4. The adjustments will be smaller and more sensitive. If adjustment of all screws in either direction lowers the output, the beam spot may be centered on the fiber core, but improperly focused.
* Turn each adjuster a small amount (1/8th turn) in the same direction, then maximize each Zθ adjuster. If the new maximum is lower than the previous, turn each Zθ adjuster a small amount in the other direction and maximize. Repeat until absolute maximum is found.

* For more information on the Thorlabs collimator, see [manual](https://www.thorlabs.com/drawings/19effe7ca9179470-EC8BF155-96AC-6091-8774197AF94FBEB8/PAF2P-A10A-Manual.pdf).

## Tips

Here are tips for some specific problems that one may encounter while assembling a DPBB.

* When IntraAction AOM shows low first pass efficiency/bandwidth, and you are quite certain that there is no issue with alignment, try flipping the AOM upside down and re-align.
* Always use broadband dielectric plane mirrors for breadboard assembly. Using mirrors with curvature may significantly reduce the fiber coupling efficiency).

# Machining notes

### Machined parts

Hole tapping requirements: the 3.302 mm tapped holes need to be #8-32 screwed, the smaller ones (2.845 mm) should be #4-40 screwed, and the larger ones (5.157 mm diameter) should be 1/4''-20 screwed.


# Double-pass breadboard overview

## 1/2" Version
<img src="https://user-images.githubusercontent.com/73464010/185268244-2909a4a2-1e7b-4073-b7e3-0711badd636a.jpg" width = "500">

<img src="https://user-images.githubusercontent.com/73464010/185266223-bcfe905a-9b51-402f-a7c5-59fe4334a190.jpg" width = "500">

## 1" Version
<img src="https://user-images.githubusercontent.com/73464010/185269233-cd3dfe01-da16-4b9c-9376-25dac20ec4bf.jpg" width = "500">




