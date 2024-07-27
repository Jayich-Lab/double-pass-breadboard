# double-pass-breadboard

The goal of this project is to realize stable, modular, and compact double pass acousto-optic modulator (AOM) systems for controlling the frequency and amplitude of laser light.  This project was directly inspired by [Ike Chuang's group](http://web.mit.edu/~cua/www/quanta/).

Breadboard versions are organized in directories labeled by the date (YY-MM) when the machined parts were *initially* ordered.  Each directory includes a README with a link to the corresponding STEP files (GitHub doesn't support the STEP file format) for the parts to be machined.


Assembled latest version (2024-04): 

<img src="https://github.com/Jayich-Lab/double-pass-breadboard/assets/101778987/368243e8-b029-4ade-aab6-5072f72cc143" width="500">



## DPBB Schematic
<img src="https://github.com/Jayich-Lab/double-pass-breadboard/assets/101778987/4fecbb3c-94f0-4d26-af58-eb430a82806f" width = "600">


## Polarizing Beam Splitter Handling

We use [Pattex Repair Extreme](https://www.pattexarabia.com/products/central-pdp.html/pattex-repair-extreme/SAP_0201OAP03X70.html) to secure the polarizing beam splitter (PBS) cubes to their mounts. 
- Note: use only a little dab of epoxy for a single corner and avoid the joint between the two halves of the cube. If epoxy contacts this joint, it will seep in over time, eventually ruining the PBS.


## Maximizing Double Pass Efficiency
* Adjust the beam path until it is level over the length of the breadboard.
* Use a beam profiler to measure the beam far away (100cm) from the input fiber port, and minimize beam divergence using the three Zθ adjusters of the [Thorlabs PAF2 Series Collimators](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=2940). 
* Adjust the height of the incoming beam so the beam passes through the center of the AOM aperture.  
* Adjust the AOM's angle using the AOM mount sliding track to maximize the diffraction efficiency at the desired AOM center drive frequency.  
* Measure the single pass efficiency and bandwidth.
* Place an plano-convex lens a focal length (f = 50 mm) away from the AOM with the convex side facing the AOM. Adjust the position of the plano-convex lens so the 0th order beam passes through the center of the lens.
* Put a flat mirror at the smallest beam width position, and adjust mirror to retro-reflect the beam. 
* Adjust the quarter wave plate and the flat mirror to maximize the light reflected back from the PBS. 
* Check the double pass efficiency and bandwidth before fiber coupling. 
* If the bandwidth is significantly smaller for the double pass, adjust the distance between the AOM and the lens to improve the bandwidth.
* Couple the light into the output fiber using the two mirrors before the output port. For detailed instructions on how to fiber couple with Thorlabs PAF2 Series collimators, see [Thorlabs manual](https://www.thorlabs.com/_sd.cfm?fileName=TTN132194-D02.pdf&partNumber=PAF2A-A10A) chapter 6.


## To-do
* Measure temperature stability.
* Test different mirror mounts.




