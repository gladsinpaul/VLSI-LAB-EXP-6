#  ANALOG DESIGN OF INVERTER, NOR AND NAND GATE USING VIRTUOSO

**AIM:** To design the following circuits using Cadence Virtuoso<br>
&emsp;&emsp;&emsp;&emsp;&emsp;1) Inverter<br>
&emsp;&emsp;&emsp;&emsp;&emsp;2) 2 Input NAND gate<br>
&emsp;&emsp;&emsp;&emsp;&emsp;3) 2 Input NOR gate<br>

**SOFTWARE REQUIRED:** Cadence Virtuoso<br>
  
**PROCEDURE**

**Commands to get into Cadence**

&emsp;&emsp;1.Right Click and open the terminal window<br>
&emsp;&emsp;2.Type the following commands as follows and press enter.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;i)tcsh<br>
&emsp;&emsp;&emsp;&emsp;&emsp;ii)source /home/install/cshrc<br>
&emsp;&emsp;&emsp;&emsp;&emsp;iii)virtuoso<br>

**Procedure for Schematic simulation using Cadence**

&emsp;&emsp;1.Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”<br>
&emsp;&emsp;2.Close the 2nd window<br>
&emsp;&emsp;3.Use 1st window i.e virtuoso window(CIW) for further processing.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;i)Create a New Library<br>
&emsp;&emsp;&emsp;&emsp;&emsp;ii)Create Schematic Cell view.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;iii)Create the Symbol for schematic Cell view.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;iv)Create the test Cell view.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;v)Analog simulation by spectre<br>

**Procedure for Creating New Library.**

&emsp;&emsp;a)File –New – Library<br>
&emsp;&emsp;b)Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK<br>
&emsp;&emsp;c)Attach the library to the technology library gpdk045.Click OK<br>

**Create Schematic Cell view.**

&emsp;&emsp;a)Go to 1st window i.e virtuoso(CIW)<br>
&emsp;&emsp;b)File-New-Cell view<br>
&emsp;&emsp;c)Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic<br>
&emsp;&emsp;d)Type: Schematic press OK<br>
&emsp;&emsp;e)Add the required components from the libraries and make the connections.<br>
&emsp;&emsp;f)Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos<br>
&emsp;&emsp;g)Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin<br>
&emsp;&emsp;h)Make the connections by using fixed narrow wire key<br>
&emsp;&emsp;i)Click Check and Save button<br>

**Creating the Symbol for schematic Cell view**

&emsp;&emsp;a.In the schematic window, execute<br>
&emsp;&emsp;&emsp;&emsp;&emsp;Crate – Cell view – From Cell view<br>
&emsp;&emsp;&emsp;&emsp;&emsp;The cell view from cell view window appears<br>
&emsp;&emsp;&emsp;&emsp;&emsp;Check Lib Name, Cell Name, From View name must be schematic Press ok<br>
&emsp;&emsp;b.Now Symbol generation form appears. Click Ok If No changes required<br>
&emsp;&emsp;c.A new window with with default symbol is created.<br>
&emsp;&emsp;d.Edit the symbol if you want to give actual symbol shape else continue.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;i.Execute Create-Cell view-from cell view<br>
&emsp;&emsp;&emsp;&emsp;&emsp;ii.Library Name and Cell Name must be same which you have used for schematic. Press OK<br>
&emsp;&emsp;&emsp;&emsp;&emsp;iii.Check for the position of pin side.Prss OK<br>
&emsp;&emsp;&emsp;&emsp;&emsp;iv.Edit for the shape by Create-Shape-Choose required options to edit.<br>

**Creating the new test cell view**

&emsp;&emsp;a)Go to CIW window, Execute File-New-Cell view<br>
&emsp;&emsp;b)Setup the new file form<br>
&emsp;&emsp;&emsp;&emsp;&emsp;Library: Select the one you a created.<br>
&emsp;&emsp;&emsp;&emsp;&emsp;Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test<br>
&emsp;&emsp;&emsp;&emsp;&emsp;View: Schematic<br>
&emsp;&emsp;&emsp;&emsp;&emsp;Type: Schematic  press OK<br>

**Analog simulation by SPECTRE.**

&emsp;&emsp;a.In test cell view window<br>
&emsp;&emsp;&emsp;&emsp;i.Launch – ADE L(Analog Design Environment)<br>
&emsp;&emsp;b.Execute Setup—Simulation/directory/Host A new window opens<br>
&emsp;&emsp;c.Set the simulation window to spectre and click ok<br>
&emsp;&emsp;d.Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.<br>
&emsp;&emsp;e.Execute Analysis – Choose. A window opens.<br>
&emsp;&emsp;f.Select the type and set the specifications and press OK<br>
&emsp;&emsp;g.Execute Output s—to be plotted – Select on Schematic<br>
&emsp;&emsp;h.Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse<br>
&emsp;&emsp;i.Execute Simulation -- Net list and Run<br>

**INVERTER:**
![330559950-f04bd811-4be9-4bb1-b6eb-7524518e8c9e](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/489994c6-77a6-4bbd-890f-f40ad0ab3bb9)

![330559968-d857149c-3a95-4704-a205-f54206683a4e](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/baf65456-87c7-4d99-bcc8-b9f730c7dbea)

**Specifications:**  
&emsp;&emsp;&emsp;&emsp;Vpulse V1 = 0,	V2 = 1<br>
&emsp;&emsp;&emsp;&emsp;Vdc	= 1<br>
&emsp;&emsp;&emsp;&emsp;td = 0,tr = tf = 1 n, ton = 100n ,T = 200n<br>


**OUTPUT:**<br>
**Simulation Settings**<br>
**Setup for transient analysis:**<br>
&emsp;&emsp;&emsp;&emsp;1.Stop time = 400n<br>
**Setup for D.C analysis**<br>
&emsp;&emsp;&emsp;&emsp;1.Component to be selected in schematic is	for d.c analysis<br>
&emsp;&emsp;&emsp;&emsp;2.Start = -1 Stop = 1 resp.<br>
**TRANSIENT ANALYSIS**
![330560340-b8234091-97b8-4b86-92c5-94566de15a02-1](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/cacb5463-d5a3-494d-bcd0-70f931b4b3eb)
**DC ANALYSIS**
![330560438-dd79284d-ad9e-4732-8f37-53ded23a0f96](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/50ceb11e-43e3-413b-9bfa-aa2d7441fd54)

**2 INPUT NAND:**<br>
![330560494-0fd4b819-3f12-49a8-86db-ad5a521c6a76](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/5b90d685-5f1e-452b-92c9-bd74512d0db4)

![330560511-1c227790-844a-43fa-923a-e5565e5fa369](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/2b7b3895-983f-4506-bdb4-8b521ace0c4a)

**Specifications:**  
&emsp;&emsp;&emsp;&emsp;Vpulse A V1 = 0,	V2 = 1,Vpulse B V1 = 0,	V2 = 1<br>
&emsp;&emsp;&emsp;&emsp;Vdc	= 1<br>
&emsp;&emsp;&emsp;&emsp;For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n<br>
&emsp;&emsp;&emsp;&emsp;For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n<br>

**OUTPUT:**
**Simulation Settings**<br>
**Setup for transient analysis:**<br>
&emsp;&emsp;&emsp;&emsp;1.Stop time =400n<br>
![330560541-71297cb2-2ef0-4eca-88f5-cde73b060e19-1](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/476464c2-d5c1-421e-8eff-6ce08ad2576f)


**2 INPUT NOR:**<br>
![330560582-38375920-7a39-4a05-8f4c-8191390b8ed3](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/8ae8ad3a-197a-4d94-9e8d-79a664e88ba5)

![330560604-2f5e04f2-e455-4d70-b8a5-84d5e44ae4c1](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/cd347672-b6ba-4800-bd2d-73736735845f)

**Specifications:** 
&emsp;&emsp;&emsp;&emsp;Vpulse A V1 = 0,	V2 = 1,Vpulse B V1 = 0,	V2 = 1<br>
&emsp;&emsp;&emsp;&emsp;Vdc	= 1<br>
&emsp;&emsp;&emsp;&emsp;For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n<br>
&emsp;&emsp;&emsp;&emsp;For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n<br>

**OUTPUT:**
**Simulation Settings**<br>
**Setup for transient analysis:**<br>
&emsp;&emsp;&emsp;&emsp;1.Stop time =400n<br>
![330560620-443361fb-04c0-4295-a69a-ddf048fd739f](https://github.com/gladsinpaul/VLSI-LAB-EXP-6/assets/117917349/8a4a31c5-9915-4d0f-8e57-3a5afcce04d1)

**RESULT:**<br>

&emsp;&emsp;Thus the analog design of inverter, nand and nor gates is done and the outputs are verified successfully.



