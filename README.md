# double-pass-breadboard

This repo tracks our double pass breadboards.  The goal is to realize reliable, modular, and compact double pass AOM systems for controlling the frequency and amplitude of laser light.  This project was directly inspired by work in [Ike Chuang's group](http://web.mit.edu/~cua/www/quanta/).

Different versions of the breadboard are organized in directories labeled by the date (YY-MM) when the parts were *initially* ordered.  Each directory includes a README with a link to the corresponding STEP files (GitHub doesn't support the STEP file format) for the parts to be machined, as well as other notes on the version.


 <image img src="./2023-03-version/2023-03-partially-assembled.jpg" width="600"></image>


<img width="599" alt="cost" src="https://user-images.githubusercontent.com/63123871/231609481-7296a951-1a45-4414-b5d5-492b8e8fb254.png">



### To-dos
* Measure performance - long-term stability, temperature stability, 



# Assembly notes

### Polarizing Beam Splitter Handling
We use [Devcon 5 Minute Epoxy](https://itwperformancepolymers.com/products/devcon-5-minute-epoxy/) to secure Polarizing Beam Splitters to their mounts. 
- Note: use only a little dab of epoxy for a single corner and avoiding line joining the two halves of the cube. If epoxy contacts this joint, it will seep in over time, eventually ruining the PBS.

### Waveplates
After the input fiber port is a quarter waveplate and a half waveplate. The waveplate after the AOM is a quarter waveplate.

### Maximizing Double Pass Efficiency
* Place the input fiber port, adjust two mirrors until the beam is completely horizontal. Use a beam profiler to observe the beam far away from the fiber port to make sure that the beam is not diverging. This step is important to get a decent efficiency on the AOM and output fiber port.
* Place the half wave plate, and a PBS on the beam path.
* Place the AOM. Adjust the height of incoming beam to let the beam pass through the aperture at the center. Keep the beam horizontal when adjusting the beam height. If the beam is too high/low, the beam will be clipped or not symmetric on the beam profiler.
* Place an iris after the AOM to select the desired defracted beam. Adjust angle of the AOM until the diffraction efficiency is highest at the frequency desired. 
Check the single pass bandwidth by changing the AOM driving frequency. Adjust the AOM to make sure that efficiency would be high enough for the frequency we are interested in. Also make sure the first order beam is not clipped and second order beam is not selected by the iris in the interested frequency range. Record the bandwidth for the single pass.
* Place an plano-convex lens (f = 50 mm used) with convex side facing the AOM after the AOM. Place it approximately its focal length away from the AOM. Adjust the height of the lens so it is at the same height of the beams. Adjust the position of the plano-convex lens so the spacing between the first and zeroth order beams is not changing after the lens. This step is crucial for getting a good double pass efficiency out of the AOM.
After finding the distance between the AOM and plano-convex lens, place the lens so the first order beam passes through the lens center. There are some references saying it would be better to let the zeroth order beam pass through center of the lens, but I (Mingyu) found aligning it with the first order beam actually improves the bandwidth.
* Place the beam profiler about a focal length away from the lens, and try to find the spot where the beam width is the smallest.
* Put a flat mirror at the smallest beam width position, and adjust the mirror so it reflects the light back into the AOM on the same path. Put a quarter wave plate before the mirror.
* Keep the first order beam selected using the iris. Adjust the quarter wave plate and the flat mirror until the light reflected back from the PBS is maximized.
* Check the double pass efficiency before fiber coupling. Check the bandwidth and it should be smaller, but comparable to the single pass bandwidth recorded in step 6.
* If the bandwidth is significantly smaller for the double pass, then adjust the distance between the AOM and the lens to improve the bandwidth.
* After the bandwidth before fiber coupling is fixed, couple the light into a fiber using two mirrors. Check the after fiber coupling efficiency. 


# Machining notes

### Machined parts

Hole tapping requirements: the 3.302 mm tapped holes need to be #8-32 screwed, the smaller ones (2.845 mm) should be #4-40 screwed, and the larger ones (5.157 mm diameter) should be 1/4''-20 screwed.
