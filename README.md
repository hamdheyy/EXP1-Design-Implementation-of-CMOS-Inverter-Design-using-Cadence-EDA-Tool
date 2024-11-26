
Ex No: 01     Design & Implementation of CMOS Inverter Design Using Cadence EDA Tools   

## Aim:
To design and implement a CMOS inverter circuit using Cadence EDA tools, analyse its electrical characteristics, and understand the fundamental principles of CMOS technology, including the design process, layout, and simulation techniques.

## Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

## Circuit Diagram :
![Screenshot 2024-11-18 230712](https://github.com/user-attachments/assets/3e30bd50-665e-4f9c-8a6d-93d564266e73)


## Schematic Simulation : 
- PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
## Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


## i)	Procedure for Creating New Library.
•	File –New – Library
<br>
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
<br>
•	Enable Attach to an existing technology library, Click OK
<br>
•	Attach the library to the technology library gpdk045.Click OK
<br>
## ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)
<br>
•	File-New-Cell view
<br>
•	Setup the new file form
<br>
•	Library: Select the one you created.
<br>
•	Cell: Give the experiment name Ex: Inverter ViewSchematic
<br>
•	Type: Schematic press OK
<br>
•	Add the required components from the libraries and make the connections.
<br>
•	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
<br>
•	Click on browse. This opens the library browser
<br>
•	Now select the appropriate library for components like 
<br>
•	Gpdk45 ------------------------nmos1v, pmos1v
<br>
•	Create Input and Output pins
<br>
•	Make the connections by using fixed narrow wire key
<br>
•	Click Check and Save button
![schematic 1](https://github.com/user-attachments/assets/5afce444-518f-4a9a-a480-332aba34319c)


 
# iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
<br>
•	Create – Cell view – From Cell view
<br>
•	The cell view from cell view window appears
<br>
•	Check Lib Name, Cell Name, From View name must be schematic Press ok
<br>
•	Now Symbol generation form appears. Click Ok If No changes required
<br>
•	A new window with with default symbol is created.
<br>
•	Edit the symbol if you want to give actual symbol shape else continue.
<br>
•	Execute Create-Cell view-from cell view
<br>
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
<br>
•	Check for the position of pin side.Prss OK
<br>
•	Edit for the shape by Create-Shape-Choose required options to edit.

 ![image](https://github.com/user-attachments/assets/e947dcda-b023-4668-a955-a5faf0949702)


## iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
<br>
•	Setup the new file form
<br>
•	Library: Select the one you created.
<br>
•	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
<br>
•	View: Schematic
<br>
•	Type: Schematic press OK
<br>
•	Follow the step 3(ii) d to make the required connections
![schematic 2](https://github.com/user-attachments/assets/96411f83-8434-48ef-a717-29dba554a7ae)


 
## Analog simulation by SPECTRE.
•	In test cell view window
<br>
•	Launch – ADE L(Analog Design Environment)
<br>
•	Execute Setup—Simulation/directory/Host A new window opens
<br>
•	Set the simulation window to spectre and click ok
<br>
•	Execute Analysis – Choose. A window opens.
<br>
•	Select the type and set the specifications and press OK
<br>
•	Execute Output s—to be plotted – Select on Schematic
<br>
•	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse

•	Execute Simulation -- Net list and Run


 ![image](https://github.com/user-attachments/assets/3aac50ec-bc0f-406e-be2e-a504b8afa8c9)
 

For Transient Analysis Settings and Output
 
 
 ![image](https://github.com/user-attachments/assets/92d14f32-8ba5-4fed-978a-38c360b8e305)

 

![transfer](https://github.com/user-attachments/assets/9cb795ab-6f1c-44a9-bb57-ef6152a05124)



 For DC Analysis Settings and Output

 
![image](https://github.com/user-attachments/assets/0ee74107-e03a-4204-b685-83ced611c993)



![dc](https://github.com/user-attachments/assets/9cd1e72b-a23f-4d70-aabe-0bc8ef64599a)

 

## Results:
1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.
3.	The Voltage Transfer Characteristic (VTC) curve was plotted, showing the relationship between input and output voltages.










