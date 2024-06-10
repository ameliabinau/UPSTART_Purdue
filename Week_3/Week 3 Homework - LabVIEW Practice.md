# Week 3 Homework - LabVIEW Practice 

LabVIEW is a software that allows for control, measurement, and manipulation of signals/data from hardware in a lab. It can also be used to program mathematical calculations and other logical flows. LabVIEW programs can be found in just about every experimental physics lab as it serves as an easy "integrator" for instrument measurements.

LabVIEW (created by National Instruments, NI) uses a "visual" programming language called G and is coded in various C languages (https://en.wikipedia.org/wiki/LabVIEW). There is a "front end" (or "front panel") to the software, where displays of information (plots, "lights" signifying binary signals, switches, buttons, numeric displays, etc.) can be created that show the status of data as it's being manipulated in the "back end" or "block diagram" of the program. 

Download LabVIEW (https://www.ni.com/en/support/downloads/software-products/download.labview-student-software-suite.html#352828) from NI. You automatically get a 45 day trial of the software. You'll have to create a NI account using your Purdue email. Once this is done and you verify your account via email, you begin the download of the LabVIEW suite. They will ask if you want to disable Windows Fast Startup; click no. Additionally, you don't want yo install any of the packages for LabVIEW and the program might take around 10 minutes to install. After it installs, your computer will restart. Launch LabVIEW when complete and click "Create Project" and "Create New VI." Every project will be called a "VI," or "Virtual Instrument." 

*Please review this introductory summary of the two different panels that are generated when you create a new project: https://learn.ni.com/learn/article/labview-tutorial*

### **Activity 1:**

Explore the "Functions" window. Name three functions from three major categories (drop-down boxes) and describe what they are used for. You can do a little research for this. 

### **Activity 2: Wein's Law Calculator**

Wein's Law is an intrinsic law of bulk materials describing the peak wavelength (m) of an object's emitted electromagnetic blackbody spectrum at a given temperature (K). Read more here: https://en.wikipedia.org/wiki/Wien%27s_displacement_law. Let's create a simple LabVIEW program that takes a numeric input (in Kelvin) and outputs the corresponding, theoretical peak wavelength in nanometers (nm). The equation for Wein's Law is: $\lambda_peak = m/T$, where m is a constant equal to about 0.002897 m*K. 

1. In your new VI, navigate to the Front Panel and find the "Controls" window. It should automatically appear when you open the VI. If it does not, go to View -> Control Palette at the top of the Front Panel. Then, in the Controls window, click on Modern -> Numeric. Under this tab, create a single Numeric Control AND a single Numeric Indicator in the Front Panel interface. Rename the Numeric Control "Temperature (K)" and the Numeric Indicator "Wavelength (nm)." The Numeric Control allows us to input some value for the temperature of our object, in Kelvin, and the Numeric Indicator will produce the result of our Wein's Law calculation once the LabVIEW program is run.

2. Navigate to the Block Diagram panel. If it is not already open, navigate to View -> Function Palette and open the Functions Window. Notice that two blocks were automatically generated when we created the Numeric Control and Indicator in the Block View -> these respresent where our input and output come in and out of our "circuit." In the Functions window, navigate to "Mathematics" and place a "Multiplication" and a "Division" operator somewhere in the block diagram. 






