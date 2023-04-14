# double-pass-breadboard

This repo tracks our double pass breadboards.  The goal is to realize reliable, modular, and compact double pass AOM systems for controlling the frequency and amplitude of laser light.  This project was directly inspired by work in [Ike Chuang's group](http://web.mit.edu/~cua/www/quanta/).

Different versions of the breadboard are organized in directories labeled by the date (YY-MM) when the parts were *initially* ordered.  Each directory includes a README with a link to the corresponding STEP files (GitHub doesn't support the STEP file format) for the parts to be machined, as well as other notes on the version.


Partially assembled 2023-03 version:  
 <image img src="./2023-03-version/2023-03-partially-assembled.jpg" width="600"></image>




# To-dos
* Measure performance - long-term stability, temperature stability, 
* Annotate a picture of a fully assembled breadboard, including laser paths to help clarify the instructions below.  
* Diagram of the double pass setup.


# Assembly notes

### Polarizing Beam Splitter Handling
We use [Devcon 5 Minute Epoxy](https://itwperformancepolymers.com/products/devcon-5-minute-epoxy/) to secure Polarizing Beam Splitters to their mounts. 
- Note: use only a little dab of epoxy for a single corner and avoiding line joining the two halves of the cube. If epoxy contacts this joint, it will seep in over time, eventually ruining the PBS.

### Waveplates
After the input fiber port is a quarter waveplate and a half waveplate. The waveplate after the AOM is a quarter waveplate.

### Maximizing Double Pass Efficiency
* Place the input fiber port, adjust two mirrors until the beam is horizontal. Use a beam profiler to measure the beam far away from the fiber port to minimize beam divergence. This step is important to get decent AOM diffraction efficiency reasonable output fiber coupling.
* Place the half wave plate and PBS in the beam path.
* Place the AOM. Adjust the height of the incoming beam so the beam passes through the aperture's center. Keep the beam horizontal when adjusting the beam height. If the beam is too high or too low the beam will be clipped or not symmetric on the beam profiler.
* Place an iris after the AOM to select the desired diffraction order. Adjust the AOM's angle to maximize diffraction efficiency at the desired AOM center drive frequency. 
Check the single pass bandwidth by changing the AOM driving frequency. Adjust the AOM to make sure that efficiency is high enough for the frequency of interest. Also make sure the first order beam is not clipped by the iris. Measure the single pass the bandwidth (and plot).
* Place an plano-convex lens, e.g. f = 50 mm, after the AOM with convex side facing the AOM. Place the lens approximately a focal length away from the AOM. Adjust the height of the lens so the beam is centered on the lens. Adjust the position of the plano-convex lens so the spacing between the first and zeroth order beams do not chang after the lens. This step is crucial for getting a good double pass efficiency.
After setting the distance between the AOM and plano-convex lens, place the lens so the first order beam passes through the lens center. There are some references saying it would be better to let the zeroth order beam pass through center of the lens, but I (Mingyu) found aligning it with the first order beam actually improves the bandwidth.
* Place the beam profiler about a focal length away from the lens, and try to find the spot where the beam width is the smallest.
* Put a flat mirror at the smallest beam width position, and adjust the mirror so it reflects the light back into the AOM following the same path. Put a quarter wave plate in front of the mirror.
* Keep the first order beam selected using the iris. Adjust the quarter wave plate and the flat mirror until the light reflected back from the PBS is maximized.
* Check the double pass efficiency before fiber coupling. Check the bandwidth. It should be smaller, but comparable to the single pass bandwidth recorded in step 6.
* If the bandwidth is significantly smaller for the double pass, then adjust the distance between the AOM and the lens to improve the bandwidth.
* Couple the light into a fiber using two mirrors. Check the after fiber coupling efficiency. 


# Machining notes

### Machined parts

Hole tapping requirements: the 3.302 mm tapped holes need to be #8-32 screwed, the smaller ones (2.845 mm) should be #4-40 screwed, and the larger ones (5.157 mm diameter) should be 1/4''-20 screwed.
