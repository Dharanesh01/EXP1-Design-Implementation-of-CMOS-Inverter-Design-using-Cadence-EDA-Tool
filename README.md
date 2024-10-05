Ex No: 01     Design & Implementation of CMOS Inverter Design Using Cadence EDA Tools   

Aim:
To design and implement a CMOS inverter circuit using Cadence EDA tools, analyse its electrical characteristics, and understand the fundamental principles of CMOS technology, including the design process, layout, and simulation techniques.

Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i)	Procedure for Creating New Library.
•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button
![WhatsApp Image 2024-10-05 at 10 30 21 AM](https://github.com/user-attachments/assets/385b7745-f3eb-4e61-bffe-4df8496a4d6a)



 
iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.

 ![WhatsApp Image 2024-10-05 at 10 30 39 AM](https://github.com/user-attachments/assets/25878c5b-d95d-40a6-96b0-afd649e97e37)



iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections
![WhatsApp Image 2024-10-05 at 10 35 56 AM](https://github.com/user-attachments/assets/7ecb400f-ac91-4a2c-9953-e4e4183e56f8)



 
Analog simulation by SPECTRE.
•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run
 ![WhatsApp Image 2024-10-05 at 10 38 24 AM](https://github.com/user-attachments/assets/78f56af6-e339-48b2-8b6f-40c2a85d7ab3)

For Transient Analysis Settings and Output
 
 
 ![WhatsApp Image 2024-10-05 at 10 39 42 AM](https://github.com/user-attachments/assets/f90aef0a-7e12-45b1-977b-553b4e493dcc)


![Screenshot 2024-09-28 115515](https://github.com/user-attachments/assets/b83ce8c9-716f-4686-bd77-3e5e0a1aec02)


 For DC Analysis Settings and Output
![WhatsApp Image 2024-10-05 at 10 42 14 AM](https://github.com/user-attachments/assets/cafabd2f-280c-4f14-9180-a5e27cd17c26)


![WhatsApp Image 2024-10-05 at 10 43 13 AM](https://github.com/user-attachments/assets/fe16799a-6392-4e29-9a35-cd2b5c2723d3)


 




 

Results:
1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.
3.	The Voltage Transfer Characteristic (VTC) curve was plotted, showing the relationship between input and output voltages.











