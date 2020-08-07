# Whack-a-Mole from Verilog
An FPGA version of Whack-a-Mole! Without a computer, users can plug in their DE1-SoC Intel FPGAs to their monitors and play an amazing game of Whack-a-Mole! Users can move hit Moles with the four button keys on the FPGA. The user can collected points for every Mole hit and loses a point for every mole missed. But the user needs to be careful; the game will be lost when he hits a special Bomb Mole! This project was made as a final course project for CSC B58: Computer Organization.

## Overview of the project
This project was made with Verilog, a hardware description language, which was used to model the electronic systems on the FPGA.

## Getting Started
The following instructions will get you run a copy of the project on Intel's DE1-SoC FPGA boards.

### Prerequisites: 
* You will need to have a physical copy of the DE1-SoC board, which can be found on https://www.altera.com/support/training/university/boards.tablet.html.

### Installing Quartus on your machine
1. 	Before you start, please check the system/memory requirements here:
	http://dl.altera.com/requirements/17.0/ 

2.	You first need to create a myAltera account here:
	https://www.altera.com/myaltera/mal-index.jsp
3. 	Once you have created your free myAltera account, you can download Quartus Prime Lite Edition 17.0 via the following link:
	http://dl.altera.com/17.0/?edition=lite.

	This download includes Modelsim-Altera.
	Downloading the combined version of the files is easier, but if you want to go the “Individual Files” route and you want to save some disk space, you can uncheck all the device families except Cyclone V; see image below:



### Compiling and running the project on the FPGA:
1. 	Open Quartus Prime (version 16) and go to File > Open Project and select /whack_a_mole.qsf.
2.  To compile the project, click Processing > Start Compilation.
3. When compilation is done, click Tools > Programmer and a window will appear.
4. Go to Hardware Setup and ensure Currently Selected Hardware is DE1-SoC [USB-x] and close the window.
5. Click Auto Detect and select 5CSEMA5 and click OK.
6. Double click <none> for device 5CSEMA5 and load SOF file (under /output_files/whack_a_mole.sof.) and device will change to 5CSEMA5F31.
7. Ensure Program/Configure for device ”5CSEMA5F31 is checked and click Start.
8. The project is now loaded on the FPGA.
