## Ex No: 05 Design & Implementation of 1 Bit Full Adder Using Cadence EDA Tools   

### Aim:
To design and implement a 1-bit full adder circuit using Cadence EDA tools and to understand its behavior in digital arithmetic operations.

### Tools Required:
-	Personal Computer
-	Cadence Virtuoso Software
  
### Circuit Diagram:

![WhatsApp Image 2024-11-13 at 16 25 39_3bc1790d](https://github.com/user-attachments/assets/d3e717a3-5b0e-4633-b599-8e824ad5c099)


### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:
  
1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
  - csh
  - source /cadence/install/cshrc
  - virtuoso   
#### Procedure for Schematic simulation using Cadence <br/>
1.	Now two windows must open <br/>
  i) virtuoso/command interpreter window <br/>
  ii) ”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.

  	   i.	Create a New Library
  	
       ii.	Create Schematic Cell view.
       
       iii.	Create the Symbol for schematic Cell view.
      
       iv.	Create the test Cell view.
     
       v.	Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
#### i)	Procedure for Creating New Library.
-	File –New – Library
-	Name: Give name for ur library Ex: VLSILAB_EXP_5
-	Enable Attach to an existing technology library, Click OK
-	Attach the library to the technology library gpdk045.Click OK
#### ii)	Create Schematic Cell view.
-	Go to 1st window i.e virtuoso (CIW)
-	File-New-Cell view
-	Setup the new file form
    +	Library: Select the one you created.
    +	Cell: Give the experiment name Ex: Inverter ViewSchematic
    +	Type: Schematic press OK
-	Add the required components from the libraries and make the connections.
    +	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
    +	Click on browse. This opens the library browser
    +	Now select the appropriate library for components like 
    +	Gpdk45 ------------------------nmos1v, pmos1v
    +	Create Input and Output pins
    +	Make the connections by using fixed narrow wire key
    +	Click Check and Save button

![Screenshot (64)](https://github.com/user-attachments/assets/6dad8d7d-320d-4e74-a2e2-e1f74e20e440)

 
#### iii)	Creating the Symbol for schematic Cell view

-	In the schematic window, execute 
     +	Create – Cell view – From Cell view
     +	The cell view from cell view window appears
     +	Check Lib Name, Cell Name, From View name must be schematic Press ok
     
-	Now Symbol generation form appears. Click Ok If No changes required
-	A new window with with default symbol is created.
-	Edit the symbol if you want to give actual symbol shape else continue.
-	Execute Create-Cell view-from cell view
-	Library Name and Cell Name must be same which you have used for schematic. Press OK
-	Check for the position of pin side.Prss OK
-	Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot (63)](https://github.com/user-attachments/assets/bdeefa96-f326-4007-8c7e-dab3659d65be)


#### iv)	Creating the new test cell view

-	Go to CIW window, Execute File-New-Cell view
     +	Setup the new file form
     +	Library: Select the one you created.
     +	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
     +	View: Schematic
     +	Type: Schematic press OK
-	Follow the step 3(ii) d to make the required connections

![Screenshot (62)](https://github.com/user-attachments/assets/3ec2640d-cca8-4181-b28d-0724224daff9)


### Analog simulation by SPECTRE.
-	In test cell view window
-	Launch – ADE L(Analog Design Environment)
     +	Execute Setup—Simulation/directory/Host A new window opens
     +	Set the simulation window to spectre and click ok
     +	Execute Analysis – Choose. A window opens.
     +	Select the type and set the specifications and press OK
     +	Execute Output s—to be plotted – Select on Schematic
     +	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
-	Execute
     + Simulation → Netlist and Run

![Screenshot (61)](https://github.com/user-attachments/assets/c5e2e21e-fb3b-4c1f-a41b-c491371130d0)


### For Transient Analysis Settings and Output
  - In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms
    
![Screenshot (65)](https://github.com/user-attachments/assets/c71d9962-c36f-4792-8171-86c8c2999585)



![Screenshot (60)](https://github.com/user-attachments/assets/212a880f-26c8-4081-90e4-a94d969def2a)



### Results:
The design and implementation of the 1-bit full adder using Cadence EDA tools were successfully completed. The simulation results verified the correct operation of the full adder, with accurate sum and carry outputs for all input combinations.
