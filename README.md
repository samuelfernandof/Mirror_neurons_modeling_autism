# Mirror-Neuron-Antunes-et-al-2017-

Modeling Mirror Neurons Through Spike-Timing Dependent Plasticity.

Model Type:	Neuron or other electrically excitable cell;

Brain Region(s)/Organism:	Neocortex;

Cell Type(s):	

Channel(s):	I Calcium; I M; I h; I Potassium; I Sodium;

Gap Junctions:	
Receptor(s):	AMPA; NMDA;

Gene(s):	Cav1.2 CACNA1C; Cav1.3 CACNA1D;

Transmitter(s):	Glutamate;

Simulation Environment:	NEURON;

Model Concept(s):	Detailed Neuronal Models; STDP;

Running NEURON model packages ============================================

The instructions below are based on the instructions for running models from ModelDB (http://senselab.med.yale.edu/ModelDB/). They assume you have installed a recent NEURON package (>7.3 is known to work), available at http://www.neuron.yale.edu.

Linux / Unix
------------
1. Download the model packages from the Downloads section. 

2. Unzip into the appropriate location

user@machine:~/dev/sim/neuron$ unzip final.zip
user@machine:~/dev/sim/neuron$ cd final

3. Launch the hoc GUI

user@machine:~/dev/sim/neuron/final$ sh run_hoc.sh


Windows
-------
1. Download one of the model packages from the Downloads section.

2. Unzip the downloaded package

3. Run mknrndll and point it to the 'mechanisms' directory inside the unzipped cell package directory

4. Run nrngui and from using 'File->working dir' menu option change to the 'mechanisms' directory. Then load the 'mosinit.hoc' script from the root of the unzipped cell package directory

5. The GUI should load automatically. Read the 'How to use the ME-type model GUI' section below

Mac OS X
--------
1. Download one of the model packages from the Downloads section, or from an me-type fact sheet. 

2. Unzip the downloaded package

3. Drag the 'mechanisms' directory inside the unzipped cell package directory onto the mknrndll.app icon

4. Run nrngui.app. Point the 'File->load dll' menu option to
mechanisms/x86_64/.libs/libnrnmech.so (You probably need to change the Filter from *.dll to *.so. Depending on your computer's processor type x86_64 might also be e.g. i686). Using 'File->load hoc' load the mosinit.hoc file in the root directory of the cell package directory.

5. The GUI should load automatically. 


How to use the ME-type model GUI
================================

There are three panels that show the output of the model. One is a graph with the membrane voltage recorded in the soma (units: ms and mV), the two other panels have a representation of the cell's morphology. The sections in the first morphology change color dependending on their membrane voltage during the simulation. When synaptic input is present, the second morphology will show the location of the activated synapses.
