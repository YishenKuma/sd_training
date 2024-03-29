# SD Training 
Content of training:
- [Day_0 : System/Tool Setup Check. GitHub ID creation](https://github.com/YishenKuma/sd_training/edit/main/readme.md#day_0--systemtool-setup-check-github-id-creation)

- [Day_1 : Introduction to iverilog design test bench](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_1--introduction-to-iverilog-design-test-bench)

- [Day_2: Timing, Hierarchical vs Flat synthesis, and Efficient flop coding style](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_2--timing-hierarchical-vs-flat-synthesis-and-efficient-flop-coding-style)

- [Day_3: Combinational and sequential optimizations](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_3--combinational-and-sequential-optimizations)

- [Day_4: GLS/Blocking vs Non blocking Assignments and synthesis simulation mismatch](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_4-timing-hierarchical-vs-flat-synthesis-and-efficient-flop-coding-style)

- [Day_5: DFT](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_5--dft)

- [Day_6: Introduction on logic synthesis](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_6--introduction-on-logic-synthesis)

- [Day_7: Basic SDC Constraints](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_7--basic-sdc-constraints)

- [Day_8: Advanced SDC Constraints](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_8--advanced-sdc-constraints)

- [Day_9: Optimization in synthesis](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_9--optimizations-in-synthesis)

- [Day_10: QOR](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_10--qor)

- [Day_11: Introduction to BabySoC](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_11--introduction-to-babysoc)

- [Day_12: BabySoC Modelling](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_12-babysoc-modelling-)

- [Day_13: Post Synthesis Simulation](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_13-post-synthesis-simulation)

- [Day_14: Post Synthesis Simulation](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_14-synopsys-dc-and-timing-analysis)

- [Day_15: Inception of EDA and PDK](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_15-inception-of-eda-and-pdk)

- [Day_16: Understand importance of good floorplan vs bad floor plan and introduction to library cells](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_16-understand-importance-of-good-floorplan-vs-bad-floor-plan-and-introduction-to-library-cells)

- [Day_17: Design and characterise one library cell using Layout tool and spice simulator](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_17-design-and-characterise-one-library-cell-using-layout-tool-and-spice-simulator)

- [Day_18: Pre-Layout STA and Importance of good clock tree](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_18-pre-layout-sta-and-importance-of-good-clock-tree)

- [Day_19: Final Steps for RTL2GDS](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_19-final-steps-for-rtl2gds)

- [Day_20: Floorplanning and Power Planning](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_20-floorplanning-and-power-planning-labs)

- [Day_21: Placement and CTS labs](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_21-placement-and-cts-labs)

- [Day_22: CTS analysis labs](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_22-cts-analysis-labs)

- [Day_23: Clock Gating Technique and Routing](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_23-clock-gating-technique-and-routing)

- [Day_24: Timing violations and ECO](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_24-timing-violations-and-eco)

- [Day_26: Introduction to mixed-signal flow](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_26-introduction-to-mixed-signal-flow)

- [Day_27: Introduction to crosstalk – glitch and delta delay](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_27-introduction-to-crosstalk--glitch-and-delta-delay) 

- [Day_28: Introduction to DRC/LVS ](https://github.com/YishenKuma/sd_training/blob/main/readme.md#day_28-introduction-to-drclvs) 

## **Day_0 : System/Tool Setup Check. GitHub ID creation**

<details><summary> Lecture Topics  </summary>

* Chip and Package
<!---
<img src="images/Chip and package.JPG" width="400">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/images/Chip%20and%20package.JPG) 

Chip: The assembly of active and passive electronic components, along with their inetrconnections, fabricated as a single unit on a thin substrate of semiconductor material.

Package: The housing that chips are placed in. The package is then either plugged into or soldered onto the printed circuit board. 

* Wire bonding
<!---
<img src="images/wire_bond.jpg" width="400">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/images/wire_bond.jpg)

Wire bonds are the interconnections between an integrated circuit (IC) or other semiconductor device and its packaging during semiconductor device fabrication.

* Core and IO
<!---
<img src="images/iopads.jpg" width="400">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/images/iopads.jpg)

Core: the section of the chip where the fundamental logic of the design is placed (Macros, IPs, Etc,.)

IO: allows the communication of data between die and external components

IO Pads: acting as gateway, connecting internal signals from the core of the integrated circuit to the external pins of the chip package

* Macros and IPs
<!---
<img src="images/macro IP.jpg" width="400">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/images/macro%20IP.jpg)

Macros: Simple custom built cell serving a sepecific funtional purpose that can be found through open sources

Foundry IPs: Macro cells developed with the intent of licencing to multiple vendor for using as building blocks in different chip designs, known as Intellectual Property 

* Communication between software and hardware
<!---
<img src="images/compilers-assemblers-translators-opener.jpg" width="400">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/images/compilers-assemblers-translators-opener.jpg) 

Compiler: reads the complete source program written in high-level language as a whole in one go and translates it into an equivalent program in assembly language

Assembler: translate the program written in assembly language into machine code represented by binary code

</details>	
	
<details><summary> Lab session </summary>

#### Steps

[Setup](https://github.com/YishenKuma/sd_training/blob/main/scripts/github_lab0.txt)

#### Results

<!---
<img src="day0.JPG" width="850">
--->
![](https://github.com/YishenKuma/sd_training/blob/main/day0.JPG) 

> error encountered after source standaloneHome/top.tcl
	
</details>	

## **Day_1 : Introduction to iverilog design test bench** 

<details><summary> Lecture + VSD-IAT recordining Topics </summary>

* RTL

RTL refers to Register Transfer Level, a design abstraction that models a circuit in terms of the flow between signals and the logical operations performed

* Verilog HDL

Verilog Hardware Description Language (HDL) is a language used to describe the behaviour of a circuit.

* RTL Deisgn

The behavioural representation of the required specification, written in verilog HDL

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/11.jpg)

RTL design is checked and verified using simulator for adherence to spec by simulatind the design

* iverilog

iverilog is the tool used for simulating the design, to verify the intent of design

the simulator acts by identifying changes in the input signal and evaluating the output based on changes identified from the input
output file dumped out is known as the vcd (value change format) file, to be viewed in gtkwave tool

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/12.jpg)

* gktkwave

gtkwave is a waveform analyzer tool primarily used for visualization

* Design

Design is the verilog code/codes which has the intended functionality meeting the required specification

* Testbench

testbench applies test vectors to the design to check its functionality

checks wether design is obeying to the required specifications

* Verilog files

design verilog file will need to have an associated testbench_design verilog file to be loaded into iverilog

design and testbench file will have a one to one coorespondance

* Library files

the library file is a collection of modules containinga a variety of standard cells

* Logic synthesis

Synthesizer is the tool used to convert RTL into a netlist

The synthesizer maps the RTL code with the digital logic circuit,using a given library file, to generate a netlist

* Netlist

Design is converted into gates and the connections are made between the gates, this file is given out as the netlist

The netlist can then be verified with the cooresponding testbench through the simulator

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/15.jpg)

* Clock timing and frequency claculation

The library file used in generating a netlist has a different sets of standards cells with variying speeds due to the combinational delay in circuit

Combinational delay in the logic path determines the maximum speed of operatiom of the logic circuit

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/16.jpg)

Because the circuit is affected by setup and hold timings, we need to have a variety usage of cells

* Setup and Hold 

Setup time refers to the time needed for data at input, to become stable before the active edge of clock

Hold time refers to the time needed for data at input, to become stable after the active edge of clock

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/17.jpg)

* Selection of cells

We need cells to work fast to meet the required performance, but will sacrifice power and area
But, to handle hold issues that may be present, we need to have cells that work slow, which will also cause circuit to be sluggish
Guidance is needed for the synthesizer to select the appropriate cells for optimum implementation of the logic circuit, this guidance is offered though the use of constraints 

</details>	
	
<details><summary>  Lab Day_1 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/1.jpg)

remote spark ubuntu terminal for coding

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/2.jpg)

cloning github repo in vlsi directory

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/3.jpg)

loading verilog files into simulator, and executing output vcd file for viewing in gtkwave

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/4.jpg)

verilog file used and corresponding testbench file used

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/5.jpg)

loading yoysy softqware to be used for synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/6.jpg)

reading library and verilog files, then performing synthesis using command "synth -top good_mux"

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/7.jpg)

generating the netlist using command "abc -liberty *lib_path*"

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/8.jpg)

shows graphical representation of realized logic

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/9.jpg)

verilog file written from netlist produced

![](https://github.com/YishenKuma/sd_training/blob/main/day_1/lab/10.jpg)

simplified verilog file written using the -noattr switch 

</details>	
	
## **Day_2 : Timing, Hierarchical vs Flat synthesis, and Efficient flop coding style** 
<details><summary> Lecture + VSD-IAT recordining Topics </summary>
* Fundamental of CMOS

complementary metal-oxide semiconductor 

used for constructing integrated circuit (IC) chips

the outputs of the PMOS and NMOS transistors are complementary to create an inverting output

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/1.jpg)

* Setup and Hold time

Setup Time is the time that the input data signals need to become stable before the active clock edge occurs

Hold Time is the time that the input data signals need to become stable after the active clock edge occurs

* .Lib

Collection of standard cells

The naming of the library includes the specific process (typical/nominal/..), temperature and voltage for the design.

The libraries created are characterized to model the variations in the process, voltage and temperature (PVT)

The variations in the process, temperature and voltage of design determines how the design will operate, and the design should be able to operate across all corners 
with the regard to difference in PVT

The library specifies on needed information for the cell mapping such as the technology, delay model, units of measurements, operating conditions , etc,.

The library holds a variety of cells along specified features of the cells such as leakage power, area, signal used for pins, and features of the cell pins.

Each combination of input that produce a unique output will have a specific leakage power.

Variations of the same types of cells will also have unique features associated.

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/2.jpg)

* Hierachical and Flat Representation

Hierarchical design shows design elements as sub-modules within “top module” rather than seeing the instantiation of gates as in flat synthesis

In a flattened “flat netlist” the hierarchies are flattened, showing all the cells used in the whole design, which is the complete structure, rather than in sub module form

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/3.jpg)

* Sub module synthesis

we perform sub module synthesis when we have multiple instances of same module, or when the design is too complex that it would be better to divide the design into sub modules to be synthesized individually

* Stacked PMOS vs Stacked NMOS

Occasionally library elements may result in the design of a stack PMOS during synthesis

This is undesirable as stacked PMOS due to its poor mobility, therefor during synthesis the logic can be restructured to use other components to create the same logic but under a stacked NMOS

E.g. use of OR gate replaced with NAND gate and INV cells

* Gltches

Glitches are unwanted pulses at the output of combinational gates

These glitches occur due to unbalanced delay to the combinational gates

The glitch at one gate can then be feed into the following component causing the later resulting output net to be extremely glitchy and causing high dynamic power consumption.

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/4.jpg)

* Flops

The presence of flops acts to shield the proceeding elements from being affected by the undesired glitch, as the clock signal is unaffected from data signals and glitches

The clock pin will allow the value to stay stable, and therefor avoid undesired glitches in the proceeding elements

The flops need to be initialized for the combinational circuit to have its desirable output

The flop is initialized through its control pins (Reset | Set)

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/5.jpg)

* Asynchronous vs Synchronous

Asynchronous flops means the output of the circuit will be triggered from the rising edge of the set/reset signal, in addition to the rising edge of the clock signal

Synchronous flops means the output of the circuit will be triggered solely on the rising edge of the clock signal, a rising edge in the set/reset pin will not prompt data to be captured

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/6.jpg)

</details>	
	
<details><summary>  Lab Day_2 </summary>

* Top module synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/7.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/10.jpg)

> Library elements used in sub modules

* flattened module synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/8.jpg)

* sub module synthsis

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/9.jpg)

* Asynchronous reset flop

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/11.jpg)

> data at q can either change at the rising egde of clock or set signal

> if set pin is toggeled high, the q will turn high as well

> when set pin is low, the q pin will be equal to d pin at the rising edge of clock signal

* Asynchronous set flop

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/12.jpg)

> data at q can either change at the rising egde of clock or set signal

> if set pin is toggeled high, the q will turn high as well

> when set pin is low, the q pin will be equal to d pin at the rising edge of clock signal

* Synchronous flop

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/13.jpg)

> q pin will only changes upon rising clock edge, and not on rising edge of reset pin

> if reset pin is high during active clock edge, then q will be set to 0

* Efficient coding style

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/14.jpg)

> no cells getting mapped during synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/Day_2/15.jpg)

> 3 bit data getting multiplied without addition cells by adding zero bit/bits or with using own data

> multiplying by 2: 111(7) + 0 = 1110(14)

> multiplying by 4: 111(7) + 00 = 11100(28)

> multiplying by 8: 111(7) + 000 = 111000(56)

> multiplying by 9: 111(7) + 00 = 111111(63)

</details>	
	
## **Day_3 : Combinational and sequential optimizations** 


<details><summary>  Lecture + VSD-IAT recordining Topics  </summary>

* Nature of synthesis and optimization

Synthesis is not a push button solution

It is dependant on the design statement and clarity of implementation

Some areas will have been applied optimization strategies, and some wont

An area or can be flagged for high effort optimization or set to don’t touch status

The more the design is affected by tool methodologies, the more likely it is to divert from the original design intent

* Optimization methodology

The synthesis tool will perform optimization by minimizing cost functions (design rule costs and optimization costs)

Cost functions vary depending on the EDA tool vendor

Optimization of a design will be an iterative process, as the results of synthesis are dependant on multiple factors such as libraries, constraints and coding styles

Optimizations costs = max delay cost + min delay cost + max power cost + max area cost (most important to least important, may vary depending on EDA vendor)

* Boolean Algebra basics

Boolean algebra constitutes a majority of the combinational optimization

![](https://github.com/YishenKuma/sd_training/blob/main/day3/1.jpg)

de morgan rule is used to transfor or gate into inverting nand gate, as or gate uses stacked pmos which is undesirable

![](https://github.com/YishenKuma/sd_training/blob/main/day3/5.jpg)

* Combinational and Sequential Optimization

Constant propagation is the simplification of a combinational circuit through boolean minimization, allowing less components to used Constant propagation occurs for both combinational and sequential logic

Synthesis optimization also allows improvement on circuit delay, as timing constraints may not be met with original logic, thus circuit is optimized by the tool to reduce gate count and minimize delay to value within expectation 

Constant propagation in combinational logic is based on Boolean algebra, whereas for sequential constant propagation, it is dependant on Boolean algebra and timing diagram analysis

![](https://github.com/YishenKuma/sd_training/blob/main/day3/2.jpg)

One of the additional optimization techniques is known as resource sharing, common inputs would be eliminated, which would also increase the number of fanouts, leaving the overall logic to be distorted in comparison to the original logic intent

![](https://github.com/YishenKuma/sd_training/blob/main/day3/6.jpg)

Boundary optimization is another technique used, where the boundaries inside top level design are optimized, the constants are pushed into and out of hierarchy, and rewires feed throughs and complementary signals

![](https://github.com/YishenKuma/sd_training/blob/main/day3/7.jpg)

Register retiming can also be done by readjusting the combinational logic, allowing the overall operating frequency to be increased

![](https://github.com/YishenKuma/sd_training/blob/main/day3/4.jpg)

State optimization is the optimization of unused gates

Cloning is a physical aware optimization that decreases the load of heavily loaded cell by replicating the cell

![](https://github.com/YishenKuma/sd_training/blob/main/day3/3.jpg)

</details>	
	
<details><summary> Lab Day_3 </summary>

#### Combinational Logic Optimization

![](https://github.com/YishenKuma/sd_training/blob/main/day3/8.jpg)

verilog files used for combinational logic optimizations

![](https://github.com/YishenKuma/sd_training/blob/main/day3/Picture9.jpg)

> evaluating the boolean logic for the first 4 verilog files

opt_check:

![](https://github.com/YishenKuma/sd_training/blob/main/day3/9.jpg)

> based on logic, an and gate is used

opt_check2:

![](https://github.com/YishenKuma/sd_training/blob/main/day3/10.jpg)

> based on logic, an or  gate is used

opt_check3:

![](https://github.com/YishenKuma/sd_training/blob/main/day3/11.jpg)


> based on logic, 3 input and gate is used

opt_check4:

![](https://github.com/YishenKuma/sd_training/blob/main/day3/12.jpg)

> based on logic, and xnor gate is used, and input b is not used for output

multiple_module_opt:

![](https://github.com/YishenKuma/sd_training/blob/main/day3/20.jpg)

> based on logic, input a is fed into submodule 1 with high pin, logic in verilog shows submodule 1 as an and gate

> the output (based on boolean should be a.1=a) will be fed as n1

![](https://github.com/YishenKuma/sd_training/blob/main/day3/23.JPG)

> sub module 2 is removed in design during "synth -top" as output n2 is not initiallised in assigned logic y = c | (b & n1)

> n1 b and c are fed into an and or gate (b and a through and gate, the output and c through or gate)

#### Sequential Logic Optimization

![](https://github.com/YishenKuma/sd_training/blob/main/day3/14.jpg)

dff_const1: 

> while reset pin is high, Q is low

> if reset toggeled to zero, q will not immediately switch to high, but only once triggered by positive edge of clock

![](https://github.com/YishenKuma/sd_training/blob/main/day3/15.jpg)

dff_const2: 

> while set pin is high, Q is high

> since input D is set high, if set is toggeled to low, the value remians high even as triggered by clock, as q = d

![](https://github.com/YishenKuma/sd_training/blob/main/day3/16.jpg)

dff_const3: 

> two flops used where the output of teh first is fed into the second

> output of first flop is similar to dff_const1

> the second flop out put stays high while set is high, once set is low, it will latch to the immdieate value of Q1, but due to delay, the value will be low, until it becomes high at the next positive edge

![](https://github.com/YishenKuma/sd_training/blob/main/day3/17.jpg)

dff_const4: 

> first flop behave similar to dff_const2, where output is high only

> second flop replicates this behaviour as well as its input Q1 is always high, so output q will also be always high

![](https://github.com/YishenKuma/sd_training/blob/main/day3/18.jpg)

dff_const5: 

> output of first flop is similar to dff_const1

> second flop also replicates the behaviour, but since its input is Q1, which toggels from low to high, Q must also toggle from low to high

> reason as to why both flops do not go high at the same time at the first positive clock edge after reset goes low, is because of the delayed capture of data at input, thus value is low until proceeding positive clock edge  

#### Unused Output Optimization

![](https://github.com/YishenKuma/sd_training/blob/main/day3/21.jpg)

Counter_opt:

> for this case, the output is assigned the final bit of count, and the first 2 bits would not have any significance on the output

> whenever count is increased, the final bit is toggeled, and since the output has no dependancies on the first 2 bits, they are unused outputs

> this case is also only using 1 dff, insetad of 3 as supposed when using 3 bit counter, but since there are 2 unused outputs, they are optimized off

> the input of flop will just be the inverted output of the flop

![](https://github.com/YishenKuma/sd_training/blob/main/day3/22.jpg)

Counter_opt2:

> in this case, our output is assigned as 3'b100

> now, we intiallize the design to use all the outputs, thus the 3 bit counter is implemented with 3 flops in the design

> we have a large amount of logic within the design for the use of the adder circuit, since the first 2 bits are used, the logic will be used

> at the output, we have inverted inputs !2!1!0, fed into a nor gate with an inverted C pin, thus the inputs are 2!1!0 ~= 3[3'b100]

</details>		
	
## **Day_4: Timing, Hierarchical vs Flat synthesis, and Efficient flop coding style** 
<details><summary> Lecture 4 & VSD-IAT recordining Topics </summary>
#### Gate level simulation

Running test bench with netlist, instead of the RTL, as Design Under Test

Since netlist is logically same to the RTL code, same test bench will align with the design

Map the appropriate technology parameters from library models at hand, to the synthesized netlist, thus allowing simulation of the netlist

Can be used in dynamic timing analysis as it can take in account various clocks and resets simultaneously, and give insight on the asynchronous performance that STA is not meant for

The reason we run GLS is to verify the correctness of design after synthesis, and ensuring the timing of design is met (GLS run with delay annotation)

![](https://github.com/YishenKuma/sd_training/blob/main/day4/1.jpg)

> https://www.electronicsforu.com/electronics-projects/gate-level-simulation-increasing-trend

#### GLS using iverilog

Design now (netlist not RTL) contains all the standard cells instantiated

Gate level Verilog models now read and given to the tool to produce the vcd file to be viewed in gtkwave

![](https://github.com/YishenKuma/sd_training/blob/main/day4/2.jpg)

#### Netlist vs Gate level verilog models

Gate level Verilog models allow for functional and timing-aware validation

The necessity in performing functional validation is due to the synthesis and simulation mismatches

![](https://github.com/YishenKuma/sd_training/blob/main/day4/3.jpg)

#### Simulation Synthesis Mismatch

* Incomplete or missing sensitivity list:  synthesizer may ignore this, but simulator will adhere to it

example case of missing sensitivity list:

![](https://github.com/YishenKuma/sd_training/blob/main/day4/4.jpg)

Simulator operates based on “activity”, if input does not change, the output will not change

Always block is evaluated only when @sel is changing

But the always block is not sensitive to the changes in i1 or i0, output y not evaluated on changes in i1 or i0, mux acts like a latch

If we want the module to be sensitive to the changes in any signal, the “always @(sel)” statement should be changed to always @(*)

* Complete sensitivity list with mis-ordered assignments (e.g. modelling sequential logic using blocking assignments) 

Example 1 of mismatch due to blocking statement:

![](https://github.com/YishenKuma/sd_training/blob/main/day4/5.jpg)

blocking statements will be executed sequentially

So for left side code, we will have 2 flops, as the values are written such that the value of d remains only at q0 until the next clock cycle

However, for the right side code, q0 is already assigned to d, so the next statement where q is q0,q will be equal to d within same cycle

This problem can be solved by using non-blocking statements, where the order of statements is not important, as the RHS will be evaluated, then LHS updated after time step, there will have to be 2 flops 

* Non standard Verilog coding

* Timing delay (e.g. placing delays on left side of always block assignments, this will not accurately model either RTL or behavioural models)

#### Blocking assignment

![](https://github.com/YishenKuma/sd_training/blob/main/day4/6.jpg)

Can be viewed as a one stop process, statements executed sequentially

The blocking assignment RHS (right-hand side equation) is evaluated, then LHS (left-hand side equation) is updated, without interruption from any other verilog statement 

Blocking assignments blocks trailing assignments in the same always blocks from occurring until after the current assignment has been completed

Temp variable is needed

#### Nonblocking assignment

![](https://github.com/YishenKuma/sd_training/blob/main/day4/7.jpg)

Nonblocking assignments can be viewed as a two step process. At the beginning of the time step, the RHS is evaluated, then at the end of the time step, the LHS is updated.

Non blocking assignments are only made to register data types and are therefore only permitted inside of procedural blocks, such as initial blocks and always blocks

Nonblocking assignments are not permitted in continuous assignments

Nonblocking operator is the same as the less-than-or-equal-to operator (“<=”)

Nonblocking assignment does not block other Verilog statements from being evaluated

#### Stratified event queue

![](https://github.com/YishenKuma/sd_training/blob/main/day4/8.jpg)

Stratified event queue defines how different events are organized into segmented event queues during simulation 

There is no priority for tasks within active event queue, the tasks can be executed in any order

![](https://github.com/YishenKuma/sd_training/blob/main/day4/9.jpg)

#### RTL coding guidelines

Blocking and nonblocking assignments in the same always block should not be mixed

Assignments to the same variable from more than one always block should not be made

Blocking assignments are meant for combinational logics

Nonblocking assignments are meant for sequential logics

Sequential and combinational logics should be kept separate

</details>									     
									     
<details><summary> Lab Day_4 </summary>
#### GLS and Synth Sim Mismatch

![](https://github.com/YishenKuma/sd_training/blob/main/day4/10.jpg)

> ternary operator: <Cond>?<T>:<F> , The execution of a parameter assign (e.g. y = x?a:b) is such that, when x is true, y =a, when x is false, y =b 

for this lab simulation, we have a mux selecting between io or i1 based on sel

as can be seen from the waveform, when sel is low, the output is set to i0 waveform

when sel is high, the output is set to i1

![](https://github.com/YishenKuma/sd_training/blob/main/day4/11.jpg)

after performing sysnthesis, we view the gate level simulation, we can see that the behaviour of the output is matching with the previous waveform

thus this case has no synthesis simulation mismatch

![](https://github.com/YishenKuma/sd_training/blob/main/day4/12.jpg)

> bad_mux

now we look at the same file, but the logic is written using an always block, and the always block is set to change whenever parameter sel undergoes change

we can see from the waveform that when sel changes, y is set to the value of i0/i1 at the point of change, but following that, it does not change and remains constant until the next change in sel

this is becuase in our code, we have not initiallized the changing behaviour of i0 and i1 into our design, thus the mux acts as a latch instead

![](https://github.com/YishenKuma/sd_training/blob/main/day4/13.jpg)

now we perform our synthesis and gate-level simulation, and we see from the waveform that now thge output y is also taking into account the changes in i0 and i1, and acts as a mux as intended

this is what is known as the synthesis simulation mismatch

this can be resolved by replacing the "always @ (sel)" statement to "always @ (*)"

 #### Synth Sim Mismatch for blocking statements 
  
![](https://github.com/YishenKuma/sd_training/blob/main/day4/16.jpg)

> blocking_caveat

for this case, the verilog is written using a blockings statement, wherein the output is set to a value of x that is only computed in the proceeding statement, meaning that the final output d is set to previous value of x, causing the output to be delayed by 1 duty cycle

as can be seen from the waveform, the output generated for d is only set in the next cycle

![](https://github.com/YishenKuma/sd_training/blob/main/day4/15.jpg)

now we have perfromed synthesis and we have our gate-level simulation

looking at the output data d, we can see that the output is not being delayed anymore, and the correct data is being displayed on the same duty cycle

there difference in the simulation clearly shows the synthesis simulation mismatch due to the use of the blocking statement

this can be solved by rearranging the order of the statements, or by using nonblocking statements

</details>	
	
## **Day_5 : DFT** 
	
<details><summary> Lecture 5 </summary>	

#### Testability

Layman terms: “A characteristic of an item’s design which allows the status (operable, inoperable, degraded) of that item to be confidently and quickly determined”

VLSI terms: “If a design is well controllable and well observable, it is said to be easily testable”

### The 3 Ws for DFT _ What, Why , Where/When

#### What:

DFT is a technique used to facilitate a design to become testable after production, or, the technique of adding an extra design to make sure it is tested after fabrication

Some examples of designs for making chips testable:

* for macros, MBist, Memory Built in self test, logic are used
* For flops, scan chains are used
* For combinational circuits, test patterns are generated, the number of test patterns will be based on the number of inputs (patterns = 2^inputs)

#### Why:

It makes testing easy at the post-production process

Chips can be tested through 3 levels after fabrication:

* Chip level, when chip is fabricated
* Board level, when chip is integrated on board or package
* System level, when several boards are assembled together

DFT is also done due to the economical and market needs, performing testing at the early stages such as chip level finding a defect in the manufacturing can prevent great loss if the fault is detected at user end, where the risk is much too high to allow, it is best to find the errors at chip level to avoid unnecessary losses

#### Where/When:

When? DFT is inserted at the beginning of design flow

Where? DFT is inserted during synthesis stage, the DFT code should be a synthesizable before being manufactured, thus it needs to be inserted during synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day5/1.jpg)

>  Asic design flow

### Pro’s and Con’s

#### Pros

* Reduces tester complexity
* Reduces tester time (70% of production of chip is due to testing time)
* Reduces chance of loss due to faulty device going to user end

#### Cons

* Adds complexity to design flow
* Increases power, area, and package pins (due to additional circuitry and pins)
* Design time will increase

### Basic Terminologies

#### Controllability

From DFT point of view, both ‘0’ and ‘1’ need to be able to propagate to each and every node within target patterns

A point is said to be controllable if both ‘0’ and ‘1’ are propagated through the scan patterns.

![](https://github.com/YishenKuma/sd_training/blob/main/day5/2.jpg)

> through the introduction of the mux for each register, we can check though the registers to see which might be faulty and causing the final output to be incorrect, insteas of testing each node one by one, this allows you better control of the design

#### Observability

To make sure each node is controllable, we need to have observability

Observability is the ability to measure the state of a logic signal

To measure a node means that the value at the node can be shifted out through scan patterns and can be observed through scan out ports

![](https://github.com/YishenKuma/sd_training/blob/main/day5/3.jpg)

> Through the usage of flip-flops, which allows the data to be observed at the output of the flops without affecting the design 

#### Fault

A physical damage/defect (fabrication defects) compared to the good system, which may or may not cause system failure

#### Error

The result of a fault, where system goes into erroneous state

#### Failure

System not providing expected service

A fault causes error which leads to system failure

#### Fault coverage

Percentage of the total number of logical faults that can be tested using a given test set T

There will be a list of checks to be made from the tests, ensuring no error is happening, the number of tests completed that are false over the total number of tests is what is known as the fault coverage

#### Defect Level

Defect level is the fraction of shipped parts that are defective, or the proportion of the faulty chip where fault is not detected and was classified to be good

### DFT Techniques

#### Ad-hoc technique

This technique needs to be done in the initial designing stages, or else it will lead to problems in the post-production stages when testing

Steps:

* Avoid combinational feedback

Raise-around condition, refers to when the output of a combinational block is feedback to its input, the signal at the input cannot be determined between the old value or the new feedback value

To mitigate that, we simply add a 1-bit register which acts as a flip flop, connected to a clokc, to ensure there will be no raise at the feedback input pin

* All flip flops must be initialized

There are cases where flip flops may go into a high impedance x-unknown state, where the output value is an unknown value x. how we can exit from this state is by resetting the flip-flops, so the set/reset pins need to be usable for the flip-flops

* Partition a large circuit into smaller blocks

Breaking large design into smaller partitions so that it can be easier to solve

* Provide test control for the signals which are not controllable

Need to add the circuitry needed to nodes to allow for the observability and controllability 

* the ATE requirements have to be considered while designing the test logic

ATE (Automatic Test Equipment) or ATGP (Automatic Test Pattern Generator) is what is used in the case where a high number of flops is used and the number of test patterns increase to a value we cannot put up manually

ATE Functionality: Scan-in phase, Parallel Measure, Parallel capture, First Scan-Out Phase, Scan-out phase

#### Structured technique 

There are a few limitations present in the ad-hoc technique, thus the structured technique was developed to improve on these limitations

* Scan

All the flip-flops are converted to scan flip-flops

* Boundary scan

Similar to scan but limited to boundary, essentially breaking the design into smaller partitions and working through them

* Built-in self-test

MBist (Memory built in self-test): Instead of designing another testable circuit for macros from scratch, the company providing the macro has already provides a built in self-test in the memory. For a macro, all the conditions will be stored in a memory, we will need to run the built in self-test to see the expected outputs based on the inputs we give. All the corner cases will be tested.

LBist (logic built in self-test): checks gates based on the logic that the component should operate on 

### Introduction to scan-chains

#### scan-chain technique

* specifying the scan constraints
* specifying scan ports and scan enables
* compiling the dft
* identifying the number of scan chains

#### scan based technique

Scan chains are elements in a scan-based design that is used to shift-in and shift-out the test data

As mentioned previously, the addition of the 1-bit register allow for observability, however we cannot have a register added to every node of logic in the design, as that would increase area used immensely

Instead, the more optimum method is to use a scan-chain, where a chain is formed by a number of flops connected back to back in a chain, with the output of one flop being connected to another

The input of the first flop is connected to the input pin of the chip (called scan-in) from where the scan data is fed. the output of the last flop is connected to the output pin of the chip (called scan-out) which is used to take the shifted data out

 Scan enable is like an enable line for the scan elements

The scan in is done using an additional mux

There are 3 types of scan lfip-flops configurations: multiplexed, clock,lssd

![](https://github.com/YishenKuma/sd_training/blob/main/day5/4.jpg)

> conversion of normal d flip-flop into muxed flip-flop, which is a scannable flip-flop

The longer the length of a scan chain, the higher the number of cycles required to shift the data in and out. 

A smaller scan chain length with same number of flops, would mean that the number of input/output ports needed as scan_in and scan_out ports are increased.

The length of the largest scan chain is determined by the number of cycles required to run a pattern. The number of ports required is twice the number of scan chains. 

The length of a scan chain can be determined through the correlation of clock cycles required during Scan In and Scan Out operations. The number of cycles required for a ATPG pattern determines th number of flip flop in the longest scan chain, thus the length of the scan chain.

#### purpose of scan flops

Main 2 reasons are:

* test the stuck-at faults in the manufactured devices, ensure that the faults can be controlled through the muxes
* test the paths in the manufactured devices for delay, to test whether each path is working at functional frequency or not.

#### Functionality of scan_chain

Goal of scan chain: to make each node in the circuit controllable and observable

Steps to perform basic scan-in and scan-out:

1. assert scan_enable (make it high) so we enable (SI -> Q) path for each flip-flop
2. keep shifting in the scan data until the intended values at the intended nodes are reached
3. de-assert_scan_enable (make it low for one pulse of clock, in case of stuck-at-testing and two or more cycles in case of transition testing), to enable the D -> Q path, so that the combinational cloud output can be captured at the next clock edge. The capture data is propagated through each register/flip-flop at every clock egde.
4. assert scan_enable once again and shift out the data through scan_out

![](https://github.com/YishenKuma/sd_training/blob/main/day5/5.jpg)

> https://anysilicon.com/overview-and-dynamics-of-scan-testing/

![](https://github.com/YishenKuma/sd_training/blob/main/day5/6.jpg)

> scan port is put in serially trough the from scan in port
> at the first clock edge, the data will be shifted in to the flip-flop, for each following data, the data will be shifted in at each clock edge. 

![](https://github.com/YishenKuma/sd_training/blob/main/day5/7.jpg)

> Capture is run at a slower frequency to detect Stuck-At faults
> Before arrival of next active clock edge, the test pattern response is processed by the combinational logic and becomes available at the D input of next flip-flop
> As soon as the active clock edge arrives, the processed test pattern response is captured by the next flip-flop and becomes available at the Q pin.

![](https://github.com/YishenKuma/sd_training/blob/main/day5/8.jpg)

> once capture is complete, the response test pattern is shifted out 
> we compare the data after it has been completely propagated to its functional data by de_asserting the scan enable, meaning the functional data is passed through
> if there is no mismatch between the output scan data and the functional data, then the combinational circuit outputs of the design are good, ensuring the registers and wires are not faulty

![](https://github.com/YishenKuma/sd_training/blob/main/day5/13.jpg) 

#### Overview of DFT compiler

![](https://github.com/YishenKuma/sd_training/blob/main/day5/14.jpg)

> DRC checks are performed before and after scan to ensure that the design rules are being violated due to the scan insertion

![](https://github.com/YishenKuma/sd_training/blob/main/day5/15.jpg)

> where synopsys-DFT comes into play

</details>
	
## **Day_6 : Introduction on logic synthesis**

<details><summary> Lecture + VSDIAT recording topics </summary>

##### takeaway from RTL course

Digital logic is a very powerful switching function used in automation and decision making

As digital logic has such a good role in performing decision making, it has become the basis for computing, electronic devices and control systems in our advancing digital world.

These specifications / behavioural models are written in HDL (Hardware Description Languages) such as VHDL or Verilog

These specifications are then represented in a programming language, which is RTL (Register Transfer Logic)

#### what is logic synthesis

In order to get the physical digital circuit that we want, we must perform synthesis, where the design is converted into gates and the connections are made between the gates, the given output file is the netlist.

This process is also known as RTL to Gate Level Translation

![](https://github.com/YishenKuma/sd_training/blob/main/day6/1.jpg)

The RTL files is used along with a .lib file to generate the netlist though synthesis

* .lib and implementation

The collection of logical modules with varying performance specifications

The .lib file consists of various flavours of gates to allow for use of gate at different operating speed, to accommodate for timing conscious circuitry (Setup and hold timings)

Faster cells allow for lesser cell delay, but the drawback is increased power and area, whereas slow cells require less power and area, but add more delay to the path

The guidance in order for synthesizer to select the appropriate cells to be used at paths is done through the constraints given

![](https://github.com/YishenKuma/sd_training/blob/main/day6/2.jpg)

The synthesized circuit can have different implementation, as the boolean logic can be restructured in various ways, meaning the synthesized circuit will have different sets of cells used, meaning the delay and paths would be different. 

The synthesis will need to produce the most beneficial implementation dependent  on the sconstraints set for the given design

The working digital logic circuit must be logically correct, electrically correct and timing met

#### Intro to DC

Design Compiler (DC) is a tool used for synthesis targeted for ASIC design flow from synopsys

Features include:

* It is a premium synthesis tool used across semiconductor industry

* Design compiler has interperability with various backend tools from synopsys, meaning it gels well with other synopsys backend tools

* Able to perform DFT scan stitch

* Can handle huge designs with extreme complexity and provide good QoR, Quality of Results

#### Terminologies associated with DC

* SDC

Synopsys Design Constraints

These industry standard design constraints are supplied to DC to guide the tool for appropriate and suitable optimization to achieving best implementation

It is used across EDA (Electronic Design Automation) implementation tools which are provided by different tool vendors

Specifies design intent in terms of the timing, power and area constraints

SDC is based on Tool Command Language, TCL

* .lib

Design library containing the standard cells

* DB

Similar to .lib, but using a different format, as DC understands libraries only in .db format. 

.lib must be converted into .db 

* DDC

Synopsys proprietary format for storing the design information

DC can write out and read in DDC

DDC has all the information loaded in the tool memory

* Design

The RTL file which has the behavioural model of the design

#### DC Setup

![](https://github.com/YishenKuma/sd_training/blob/main/day6/3.jpg)

#### Implementation Flow of ASIC

The steps in converting RTL to the Physical Database, GDS format

![](https://github.com/YishenKuma/sd_training/blob/main/day6/4.jpg)

#### DC Synthesis Flow

![](https://github.com/YishenKuma/sd_training/blob/main/day6/5.jpg)

#### TCL basics

TCL is the language used for writing the sdc files

All the dc internal commands are based on TCL only 

* set

Create and store information in variables

Square brackets are used for nesting the commands in TCL

![](https://github.com/YishenKuma/sd_training/blob/main/day6/6.jpg)

The variables can be shown using echo $"variable"

The "$variable" cannot be used during set, it must be set variable

* if {condition} {statement} else {statement_2}

Executes statement only if condition is true, else executes statement_2

![](https://github.com/YishenKuma/sd_training/blob/main/day6/7.jpg)

* while {condition} {statement}

Enters a repetitive loop to executing statement as long as the condition is met

![](https://github.com/YishenKuma/sd_training/blob/main/day6/8.jpg)

Incorrect writing of the while loop can lead to infinite loop, as condition may be written in such a way that the condition is always true

![](https://github.com/YishenKuma/sd_training/blob/main/day6/9.jpg)

* for {looping var} {condition} {looping var modification} {statement}

Executes a statement if condition is met based on the looping variable set , and executes until the condition is no longer met due to the looping var modifications in each iteration of loop

![](https://github.com/YishenKuma/sd_training/blob/main/day6/10.jpg)

* foreach var list {statements}

Executes command for every element present in the variable list

![](https://github.com/YishenKuma/sd_training/blob/main/day6/11.jpg)

* foreach_in_collection var collection {statements}

Specific to synopsys tools

Excecutes command for each element in the collection , similar to list, but returned by many dc commands

![](https://github.com/YishenKuma/sd_training/blob/main/day6/12.jpg)

</details>
	
<details><summary> Lab Day_6 </summary>
	
#### Invoking DC basic setup

![](https://github.com/YishenKuma/sd_training/blob/main/day6/13.jpg)
 
> Cloning github files into unix environment

![](https://github.com/YishenKuma/sd_training/blob/main/day6/14.jpg)

> loading dc_shell

![](https://github.com/YishenKuma/sd_training/blob/main/day6/15.jpg)

> The tool points to your_library.db library file, which is an imaginary non-existent library file, a dummy library pointed to in dc

![](https://github.com/YishenKuma/sd_training/blob/main/day6/16.jpg)

> verilog file used for synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day6/17.jpg)

> Theoretical logic representation of verilog file 

![](https://github.com/YishenKuma/sd_training/blob/main/day6/18.jpg)

> reading the library file

Dc will load internal dbs in the dc memory to infer the design first

The tool will try to understand the design using gtech

It invokes HDL compiler as the codes used are written in verilog

The warning given, cant read link_library is because the dummy variable is not set to any real variable, we must initialize the variable appropriately

Once the source file is compiled the registers are inferred

The register inferred is a I bit flip flop with AR (asynchronous reset)

![](https://github.com/YishenKuma/sd_training/blob/main/day6/19.JPG)

> written netlist not linked with sky123 lib, but instead using virtual libraries

Internal virtual libraries have been inferred in the netlist after the input and output have been declared

These libraries are known as GTECH, they are used since no proper library path was declared for the design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day6/20.jpg)

> GTECH is still being used instead of the sky libs, the reason for this is because the 2 variables $link_library and $target_library has not been set

![](https://github.com/YishenKuma/sd_training/blob/main/day6/21.jpg)

> The star signifies the libraries that are already in DC memories, as we do not want to override them, we do not want to lose any libraries that may be used by the tool

![](https://github.com/YishenKuma/sd_training/blob/main/day6/22.jpg)

> Now the tool can link the sky lib for performing synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day6/23.JPG)

> Running compile command

![](https://github.com/YishenKuma/sd_training/blob/main/day6/24.JPG)

> Now we can see that the netlist is no longer using GTECH and is using the components from the sky130 lib file

#### ddc gui with design_vision

![](https://github.com/YishenKuma/sd_training/blob/main/day6/25.JPG)

> A ddc file must be written out to be viewed by the design_vision tool

![](https://github.com/YishenKuma/sd_training/blob/main/day6/26.JPG)

> Exit and use command "design_vision" to invoke tool to view design

![](https://github.com/YishenKuma/sd_training/blob/main/day6/27.JPG)

> Read the ddc file in the design_vision tool

![](https://github.com/YishenKuma/sd_training/blob/main/day6/28.JPG)

> We cannot read the verilog file written "lab1_flop_net_3.v", the library path will be set to the GTECH paths, as this command will only read the verilog file 

![](https://github.com/YishenKuma/sd_training/blob/main/day6/29.JPG)
 
> Reading the ddc file allows the library paths to be included into the tool when read, as the ddc file saves all information in the tool memory during the used session

![](https://github.com/YishenKuma/sd_training/blob/main/day6/30.JPG)

> The advantage of using the ddc file is that ddc is Synopsys propriety format, meaning that it can only be read by synopsys tools, so we can write the ddc file from DC and hen read it in ICC tool

![](https://github.com/YishenKuma/sd_training/blob/main/day6/31.JPG)

> Viewing the schematic of the design, double clicking the module allows to view all the standard cells present

![](https://github.com/YishenKuma/sd_training/blob/main/day6/32.JPG)

> Schematic is matching with the verilog file read, only difference to note is the inverter connected to the reset pin, however, this is due to the flop reset pin being active low

#### dc synopsys dc setup

Every time we open DC, the 2 variables need to be set

set target_library DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db

set link_library {* $target_library}

This is a very tiresome and error prone disadvantage with using this process

The solution to this is though the use of .synopsys_dc.setup 

There will be 2 versions of this file, one in the DC installation area, and one in the DC home area

One advantage that DC flexibility offers is that DC will pick the .synopsys_dc.setup file if it is present in the home directory before looking to the installation directory, so we can make changes to the file in the home directory to perform the repetitive tasks for tool setup, meaning we will not have to manually set the target_library and link_library each time dc is invoked

![](https://github.com/YishenKuma/sd_training/blob/main/day6/33.JPG)

> Writing a .synopsys_dc.setup file to be used by dc during invocation

![](https://github.com/YishenKuma/sd_training/blob/main/day6/34.JPG)

> Now we can see that the target_library and link library have already been set because it was read from the .synopsys_dc.setup file

![](https://github.com/YishenKuma/sd_training/blob/main/day6/35.JPG)

> If we alter the file naming even slightly, it may not be picked up by the tool

![](https://github.com/YishenKuma/sd_training/blob/main/day6/36.JPG)

> Now that the naming is not correct, the commands are not read and thus dc tool library path will once again be set to their imaginary paths

#### tcl scripting

![](https://github.com/YishenKuma/sd_training/blob/main/day6/37.JPG)

> Usage of set and for loop commands

![](https://github.com/YishenKuma/sd_training/blob/main/day6/38.JPG)

> Performing arithmetic using expr to perform calculation on variable

![](https://github.com/YishenKuma/sd_training/blob/main/day6/39.JPG)

> Usage of while loop

![](https://github.com/YishenKuma/sd_training/blob/main/day6/40.JPG)

> Usage of foreach loop

![](https://github.com/YishenKuma/sd_training/blob/main/day6/41.JPG)

> Difference to note between list and collection is that elements in a collection will be printed within brackets {}, a collection is a synopsys propriety format

![](https://github.com/YishenKuma/sd_training/blob/main/day6/42.JPG)

> Usage of foreach_in_collection 
 
</details>
	
## **Day_7 : Basic SDC Constraints**

<details><summary>  Lecture + VSDIAT recording topics </summary>

#### Intro to STA

##### Max and Min delay Constraints

![](https://github.com/YishenKuma/sd_training/blob/main/day7/1.jpg)
 
The max frequency that this path can operate on can be used to set the constraint the max delay that the combinational circuit must be. The signal launched from DFFA on clock edge should reach DFFB setup time before next clock edge.

The maximum time the combinational circuit takes including setup time of flop b must be less than the time period of clock received by both flops.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/2.jpg)

The min delay constraint is just as important as having the max delay constraint. For circuit to work properly, the signal launched by DFFA on clock edge should reach DFFB only after hold time has passed after the clock edge.  

The minimum delay of combinational circuit must be greater than the hold time of DFFB , as the data should not change within the hold window.

##### Delay

![](https://github.com/YishenKuma/sd_training/blob/main/day7/3.jpg)

We can use the water bucket analogy to explain the importance of delay. The aim is to fill the bucket with water.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/4.jpg)

The time taken is determined by the inflow, the lower the inflow, the higher the time needed.

In digital logics, the time for the gate to go from 0 to 1 is determined by the delay, the lower the inflow, the higher the delay. In terms of digital logics, the inflow of water is equivalent to the inflow of current, or the input transition, the lower the input transition, the higher the delay in circuit.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/5.jpg)

Now we look at the analogy with the same inflow for both cases, but the size of the bucket is larger for case 1

![](https://github.com/YishenKuma/sd_training/blob/main/day7/6.jpg)

The larger the size of bucket, the longer the time taken to fill bucket. In terms of digital logic, delay is a function of load capacitance, the higher the load capacitance, the higher the delay.

High delay can come from either low input transition into gate, lengthy nets, or nets with high fanouts. Delay of cell will be a function of input transition and output load. We can attempt to reduce delays caused by these issues by either upsizing cell to increase input transition, or shorten the length of route between elements, or inserting buffers in between to reduce the load.

##### Timing ARC

* Combinational Cell

The delay information from every input pin to every output pin which it can control is present in the timing arc

![](https://github.com/YishenKuma/sd_training/blob/main/day7/7.jpg)

In the case of this mux, the output y is dependant on the 3 input pins i0, i1 and y, thus there will be 3 timing arcs, as the change in any of the input pins can cause a change in the output pin

* Sequential Cell

![](https://github.com/YishenKuma/sd_training/blob/main/day7/8.jpg)

For flip-flops, the delay information from clock to Q will be present in the timing arc, as the output can only change based on the change in clock

For latch, the delay from clock to Q, and the delay form D to Q will be present in the timing arc, as the output may change based on change in either clock or D

We also have setup and hold time requirements

![](https://github.com/YishenKuma/sd_training/blob/main/day7/9.jpg)

1 matter to note is that the setup and hold does not occur from pos level clk for PosLevelDlat, and neg level clk for NegLevelDlat. Setup hold is around the sampling point of the clock. There is a distinct difference in the sampling point for pos/neg edge DFF and Pos/Neg level Dlat. The sampling edge will occur at the point before data becomes opaque while still transparent.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/10.jpg)

##### Timing Paths

![](https://github.com/YishenKuma/sd_training/blob/main/day7/11.jpg)

The timing path is the path between the start point and end point, where start point is the input port or clock pin of sequential element, and end point is the output port or D pin of sequential element

![](https://github.com/YishenKuma/sd_training/blob/main/day7/12.jpg)

In this example, we are having 2 timing paths with delay of 1.7ns and 1.2ns respectively.

Based on the previous discussion, we can derive an equation for max delay Tck, which is,

Tck => Tcq + Tcomb +Tsetup

TckA => 0.5 +1.2 + 0.5 => 2.2ns [Critical Path]

TckB => 0.5 + 0.7 +0.5 => 1.7ns

TckA is having a higher value of max delay, thus it becomes our critical path, and our frequency will be defined on this value

Fclk = ½.2ns = 454.5Mhz

We can achieve a better frequency in this circuit by improving the delay on the critical path, the way we can do this is by setting constraints on the elements to limit the value of delay

#### Constraints

In setting constraints for the design, we must first establish how much delay is acceptable.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/13.jpg)

In practice, we have a desired frequency for the circuit to operate on, thus we need to calculate the acceptable delay based on this. We must squeeze the combinational logic delay such that the desired frequency is achievable.

Once the clock period is defined, the synthesis will work to optimize the logic based on the clock period, and the delays between the reg to reg paths will be limited, and the appropriate cells will be selected form the libs to meet the delay needed.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/14.jpg)

Now if we look from a bigger picture, we are having more reg to reg paths as the number of elements begin to become more complex outside a boundary. These are synchronous paths, and thus the input and outputs needs to be constrained as well to squeeze the delay.  

* Reg to Reg is constrained by clock ( Tck => Tcq + Tcomb + T su)

* Reg to Out is constrained by Output external delay and clock period

* In to Reg is constrained by Input external delay and clock period

The Reg to Out and In to Reg are called IO paths and the delay modelling referred is called IO delay modelling. IO delay modelling is usually based on STD interface specifications

we must set the constraint on the external delay because we are having 2 unknown delays from the internal combinational logic and the external, thus we can split the available time between the 2 through constraining the external delay

In handling constraints, we must be aware of the budget of the design for external module, and collect all the necessary information in planning the synthesis, so that we can understand properly and create good constraints.

#### INP Trans Output Load

If we look at our case at an idealistic perspective, the IO Delay modelling should be sufficient for setting the delays to allow for desired frequency

![]( https://github.com/YishenKuma/sd_training/blob/main/day7/15.jpg)

However, our signals are not always ideal, as signals do not have zero rise time, thus input transition is playing a role in creating delay that was not accounted, thus we must model our input transition delay as well, which will further squeeze the logic so that the timing is met

![](https://github.com/YishenKuma/sd_training/blob/main/day7/16.jpg)
 
The next thing we need to consider is the output load, as the cell delay affected by it, and if we do not take into and model the load, then the output logic will behave differently, as this is a parasitic net, not an ideal net. Thus, the logic needs to be squeezed further again to factor in the output load. General rule is to set 70% of timing for external delay and 30% for internal delay.

The value that needs to be modelled for the input transition and output load is determined by the spec. if in the case that the external input and outputs are interfaces at the chip boundary, then the interfaces would have specifications that can determine value of load 

If we have 2 models that are synthesized separately, we can perform the budgeting by discussing with the module owners to set the appropriate constraints

We need to have an optimum budgeting for setting the constraints, as under-budgeting causing setup violations, and over-budgeting may lead undesired effects such as high leakage power and high area consumption

#### Timing dot Libs

We have mentioned previously that the .db is what is used by the tool for reading the lib for the design. We cannot read the .db, however we are able to read the .lib file to understand the information present and how the tool infers the information.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/17.jpg)

Aside from the information discussed preciously that can be found in the .lib such as PVT settings and unit for current, power, voltage ,.etc, we can also find the max transition and max capacitance.

Max transition refers to the maximum slew that is allowed at the input pin of cell.

Max capacitance refers the maximum allowed capacitance on the output pin of a cell.

These 2 are used as a last line of defence to model the design in such a way to control the capacitances and transition times. For example, for high fanout out nets that would accumulate high capacitance, the tool will perform buffering on the nets so that the capacitance at the output pin does not violate the max capacitance set. Users are able to manually set the values for max capacitance and max transitions to constrain the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/18.jpg)

As mentioned before, delay is a function of input transition and output load

![](https://github.com/YishenKuma/sd_training/blob/main/day7/19.jpg)

The library provides a table for every cell specifying the input trans and output load and the resulting delay. The tool will be able to know the input trans and output load for each device imported from libs based on the lookup table. 

![](https://github.com/YishenKuma/sd_training/blob/main/day7/20.jpg)

However, the lookup table cannot specify all the values that me be used, thus there may be interpolation done for the values in between data in lookup table to acquire an accurate value.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/21.jpg)

The lookup table is not limited to delay, it can be used for getting data for multiple other specifications in the lib.

Each cell will be having varying flavours meaning different drive strength, cell area, leakage power, pin capacitance, max allowed transition per pin. Functionality and assignment of pins are also shown in the ./lib, known as attributes The data in the .lib is also specified for power and timing factors separately. The tool understands the connections and assignments of cells through the attributes specified in the lib.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/22.jpg)

Unateness refers to the behaviour of cell as a rising input is fed through. Positive unate is when the rising input results in a rising output or no change in output. Negative unate is when the output is the inverted version of input logic. Non-unate refers to when the positive unateness and negative unateness is seen from a cell.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/23.jpg)

Unateness is important as the tool uses the information to propagate the transition.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/24.jpg)

For sequential cells, the timing sense can differ based on the rising or falling edge, as Q may be rising or falling with respect to clock.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/25.jpg)

The setup timing for posedge and negedge flops will be known by the tool from the data that is given from the lib file, as this information is present as written for the specific timing type

![](https://github.com/YishenKuma/sd_training/blob/main/day7/26.jpg)

The related pin also shows the appropriate edge that the timing type should be, as “_N” refers to the inverted state of pin, thus as can be seen above, the timing type for CLK_N is setup_falling while for CLK it is Setup_rising.

![](https://github.com/YishenKuma/sd_training/blob/main/day7/27.jpg)

For latches, as we mentioned before, the pos latch will sample the data on negative edge before opaque state, whereas for Neg latch, data will be sampled on the rising edge

![](https://github.com/YishenKuma/sd_training/blob/main/day7/28.jpg)

The tool can get this data from the lib file as well.

This info present in the .lib tells the tool what to do for setup calculation during specific egdes.

</details>
	
<details><summary> Lab day 7 </summary>

Querying the properties of .lib from dc shell 

* list_lib 

![](https://github.com/YishenKuma/sd_training/blob/main/day7/29.jpg)

> shows the libraries that have already been loaded

* get_lib_cells

![](https://github.com/YishenKuma/sd_training/blob/main/day7/30.jpg)

> query all the and gates in the library

* sizeof_collection

![](https://github.com/YishenKuma/sd_training/blob/main/day7/31.jpg)

> displays number of collection queried

* foreach_in_collection

![](https://github.com/YishenKuma/sd_training/blob/main/day7/32.jpg)

* get_lib_pins

![](https://github.com/YishenKuma/sd_training/blob/main/day7/33.jpg)

* get_attribute

![](https://github.com/YishenKuma/sd_training/blob/main/day7/34.jpg)

> foreach_in_collection x [get_lib_pins sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand4b_4/*] {echo [get_object_name [get_lib_pins $x]] "="  [get_attribute [get_lib_pins $x] direction]} 

> command prints pin names with associated direction

* get_lib_attribute

![](https://github.com/YishenKuma/sd_training/blob/main/day7/35.jpg)

> foreach_in_collection x [get_lib_pins sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand4b_4/*] {echo [get_object_name [get_lib_pins $x]] "="  [get_lib_attribute [get_object_name [get_lib_pins $x]] direction]}

> command prints pin names with lib associated direction

![](https://github.com/YishenKuma/sd_training/blob/main/day7/36.jpg)

> foreach_in_collection x [get_lib_pins sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand4b_4/*] {echo [get_object_name [get_lib_pins $x]] "="  [get_lib_attribute [get_object_name [get_lib_pins $x]] function]}

> command prints pin names with lib associated function

> 4 input nand gate should show !A|!B|!C|!D , in our run the !A is replaced with A_N meaning inverted pin

* script to filter pins by output pins and show function

![](https://github.com/YishenKuma/sd_training/blob/main/day7/37.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day7/38.jpg)

* get_lib_attribute $cell area

![](https://github.com/YishenKuma/sd_training/blob/main/day7/39.jpg)

* get_lib_attribute $input_pin capacitance

![](https://github.com/YishenKuma/sd_training/blob/main/day7/40.jpg)

* get_lib_attribute $input_pin clock

![](https://github.com/YishenKuma/sd_training/blob/main/day7/41.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day7/42.jpg)

* get_cells -filter

![](https://github.com/YishenKuma/sd_training/blob/main/day7/43.jpg)

* list_attributes

![](https://github.com/YishenKuma/sd_training/blob/main/day7/44.jpg)

</details>
	
## **Day_8 : Advanced SDC Constraints** 
 
<details><summary> Lecture + VSDIAT recording topics </summary>

#### Clock Tree Modelling - Uncertainty

What needs to be constrained for clock? Our constraint on the clock will resukt in the constraint on the combinational delay. But is constraining the clock period all that is needed?

The clock arriving at a flop will most of the time never reach the next flop at the same time. This is because the distance n routing will not be the same, thus the time will be different, in order to make up for this, the clock path is buffered in order to ensure the clock arrive at same time, but it will not be exact. The slight differences in arriving time for clock in practical networks will affect our timing. 

![](https://github.com/YishenKuma/sd_training/blob/main/day8/1.jpg)

> clock generation

All our clock sources will also have inherent variations in the clock period due to stochastic effects. There will be non-zero rise time, and the edge will arrive within a window, wherein the location of edge varies from cycle to cycle within window. This is known as jitter,  meaning edge will arrive within a margin window and not at the exact time as expected.

Because of this jitter, our timing will not be as expected as our margin will not be the same anymore.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/2.jpg)

> clock distribution

Practical clock networks after CTS stage may not see the clock edges at the same instance. The indifference in clock distribution networks between components is known as clock skew. CTS will try to balance the clocks and bring the value of clock skew to as close to 0 as possible.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/3.jpg)

 > clock skew 

Tclk => Tcq + Tcomb + T su + Tskew (our timing delay now affected by the clock skew)

During synthesis, our timing will be clean, but once CTS is performed and the delays and clock skews are introduced, our available timing window will be eaten up. Thus we need to perform optimization with consideration to clock skew and jitter (duty cycle or period jitter).

* Duty cycle jitter: The variation in timing from one rising clock edge to the following falling clock edge, also referred to as Ton/Tperiod

* Period jitter: The variation in timing from one rising clock edge to the following rising clock edge

Clock skew and Jitter are known as clock uncertainty

In addition to that we need to factor in the source latency and the clock network latency also.  The source latency refers to the time taken by the clock source to the generate clock. Clock network latency refers to the time taken by the clock distribution network. 

Any modelled clock skew and latency should be removed post CTS , as the actual clock tree delay should be calculated by the tool. The pessimism needs to be removed from the constraints.

Stage | Clock Uncertainty 
--- | --- 
Synthesis | Jitter + Skew 
Post CTS | Only Jitter 

#### IO delays

Ports are the primary IOs of the design for the inputs and outputs. We can query the ports of the design using “get_ports”, and the selection can be filtered through various was. Keep in mind that the attributes will be case sensitive.

We use the commands set_input_delay and set_input_transition on our input ports to constrain the IO paths..

* set_input_delay -max 3 (allows the data to take a max of 3 ns to arrive)

* set_input_delay -min 0.5 (data may come as early as 0.5ns)

Similarly for output ports, we need to use the command set_output_delay and set_output_load for constraining the IO path.

* set_output_delay -max 3 (allows the data to take a max of 3 ns to change)

* setoutnput_delay -min 0.5 (data may change as early as 0.5ns)

The command used to create the clock is “create_clock” with an associated name and period on a valid clock definition point, the clock should not be created on the hierarchical pins which are not clock generators. The clock must be created on either generated clocks (PLL, OSCILLATORS) or primary IO pins.

![]( https://github.com/YishenKuma/sd_training/blob/main/day8/7.jpg)

If we want our clock waveform to have a starting low phase, or start at a different time, then we need to add the option to the create clock command “-wave {first_rise_edge and first_fall_edge}”

In order to bring in the practicalities of the clock network, in addition to the create clock command, we need to also set that clock latency “set_clock_latency”, which models that clock delay, and set the clock uncertainty “set_clock_uncertainty”, to set the skew and jitter of clock. Later this needs to be modified such that it only reflects the jitter once the clock tree is built. 

#### Generated clocks

 We also need to note that while the Output is being constrained with the clock leaving the module, we are not taking into account the physicality of the clock leaving the module, as the routing length would be increased, we should be experiencing more delays on the path. This is known as the propagated delay. The way we handle this is using generated clocks.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/35.jpg)

We do this using the command “create_generated_clocks” which needs to be with respect to the master clock. The -master and -source options will tell us what is the source with respect to what  the clock is created. The generated clock may be having a division factor as well, which divides the master clock by a factor.  -div 1 tells us that there is no clock divider in the circuit. 

The output needs to be constrained with respect to output clock and not the input clock, so we need to set our output delay for the output clock. The riming at the output needs to be met with respect to the output clock.

Given a case scenario in which we are having 2 different clocks coming from a mux propagated through the design, DC tool will not propagate the clocks based on the intent of the designer but based on the timing arcs that are presented in the design. All the timing arcs from the definition point will see the clock propagation by default, which is undesirable. We need to specify in the design such that the clocks propagate according to the intent of the designer through the desired paths and that this is understood by tool.

#### Vclk, Max Latency, Rise_fall, IO delays

* input delay

![](https://github.com/YishenKuma/sd_training/blob/main/day8/42.jpg)

Set input delay will cause the clock to be shifted left by the specified time for -max. The available time will be equal to the clock period – uncertainty – input delay. If the value for max is a negative value, then the clock will be shifted to the right, making the available time increase. Positive delay tightens while negative delay relaxes the timing.

Set input delay will cause the clock to be shifted left by the specified time for -min. This will be good for hold, as the window for data to be captured is increased. If we have no min delay, we might be violating on the hold timing. However, if we have a negative value for the delay, and the clock is shifted to the right, then the data would not be captured in the appropriate clock cycle. Positive delay will relax while negative delay tightens hold timing

> This behaviour is similar for set output delay. 

If we are having a data path fed into the input of our port, but it is operating on negative edge of the clock, the way we can add this constraint in addition to other constraint specified is through the options -add, and the option -clock_fall so the tool knows that the delay specified is in regard to the falling edge and not rising edge of the clock. The advandtage of using both constraints is that the design can be optimized appropriately depending on the design. 

> This behaviour is similar for set output delay. 

* Virtual Clock

If  we are having a path purely on combinational logic, then we can constrain the path simply by using the set max latency command from input port to output port. 

We can also constrain the design through the use of virtual clocks, for paths which are purely combinational logic. In system level, the path is looked at as external reg to reg path with an actual clock, so if the logic is not optimized appropriately, the path will suffer in the top implementation. Virtual clocks are created with no defined point, as long as no definition point is specified, the clock will be a virtual clock. Then we can set the constraints on the ports through this virtual clock.

> since the virtual clock is an imaginary clock, there is no latency.

* Driving cell

When we have our transition delay, and it passes through the circuit it is going to be come more delayed due to the heavy load. In reality, the transition will get degraded when it sees a load, this is because it will be driven by another cell. Instead of blindly modelling the transition, if we model the cell driving the port, the characteristics of the cell will change depending on the load. 

If we model an input transition, this transition will be a fixed transition irrespective of the load. But the transition will get worse if the load is heavier, thus we can use set_driving_cell to handle the variation in transition due to load. Set driving cell is more accurate and recommended for all internal paths.

For top level primary IOs, we should use set input transition. For module level IOs, we should use set driving cell. Set driving cell is preferable mainly because it is a more realistic approach. This is just the recommended approach, as long as we can model the real behaviour of the silicon during implementation, there is no issue.

</details>
	
<details><summary> Lab day 8 </summary>
	
#### get cells, get ports, get nets

![](https://github.com/YishenKuma/sd_training/blob/main/day8/5.jpg)

> Verilog file used for lab, in which 3 flops are used with combinational logics are used between the flops

![](https://github.com/YishenKuma/sd_training/blob/main/day8/6.jpg)

> 3 registers read in design

![](https://github.com/YishenKuma/sd_training/blob/main/day8/9.jpg)

> schematic of design from design_viewer
![](https://github.com/YishenKuma/sd_training/blob/main/day8/8.jpg)

> get cells and ways of usage

> hierarchical cells refer to cells that do not physically exist

> ref_name will not be the same as the instance_name as the ref_nam is based on the definition in the lib file

![](https://github.com/YishenKuma/sd_training/blob/main/day8/4.jpg)

> get ports and ways of usage

![](https://github.com/YishenKuma/sd_training/blob/main/day8/10.jpg)

> get nets and ways of usage

![](https://github.com/YishenKuma/sd_training/blob/main/day8/11.jpg)

> one thing to keep in mind in regards to nets is that you cannot have 2 driving pins into 1 driven pin, the reason for this is because it create corrupted logic on the node, this is known as a multidriven net
#### get pins

![](https://github.com/YishenKuma/sd_training/blob/main/day8/12.jpg)

> Get_pins and ways of usage

![](https://github.com/YishenKuma/sd_training/blob/main/day8/13.jpg)

> one thing to note for the clock attribute for pin is that the attribute is only set for input pins, if we use the command for output pins we will receive an error

> another attribute to distinguish is clocks which will list out the name of clock connected to the CLK pin, whereas for clock, it is shows pins that have been specified for clock input by true or false

![](https://github.com/YishenKuma/sd_training/blob/main/day8/14.jpg)

> for our lab presently, we do not have any clocks created yet, so we will need to use the create_clock command to do this

#### create clock waveform, , get clocks, querying clocks

![](https://github.com/YishenKuma/sd_training/blob/main/day8/15.jpg)

> now we have generated a clock for the clock pins

![](https://github.com/YishenKuma/sd_training/blob/main/day8/17.jpg)

> the attribute for is_generated is set false meaning that the clock is the master clock

![](https://github.com/YishenKuma/sd_training/blob/main/day8/16.jpg)

> reporting the clocks

![](https://github.com/YishenKuma/sd_training/blob/main/day8/18.jpg)

> getting the name of clocks connected to input pins

![](https://github.com/YishenKuma/sd_training/blob/main/day8/19.jpg)

> creating bad clock

![](https://github.com/YishenKuma/sd_training/blob/main/day8/20.jpg)

> incorrect placement for clock as this will create a broken logic. We can use command “remove_clocks” to remove the enwanted clock

![](https://github.com/YishenKuma/sd_training/blob/main/day8/21.jpg)

> we can create clocks with different waveforms as discussed earlier using the -waveform option to specify the first rise_edge and first fall edge 

#### clock network modelling – uncertainty, report timing

Uncertainty refers to the clock skew and jitter

![](https://github.com/YishenKuma/sd_training/blob/main/day8/22.jpg)

> Setting the source, and network latency, and the clock uncertainty for setup and hold times

![](https://github.com/YishenKuma/sd_training/blob/main/day8/23.jpg)

> if we report timing without any clocks created, we will have an unconstrained path

![](https://github.com/YishenKuma/sd_training/blob/main/day8/24.jpg)

> once the clock is constrained, we can see if the timing is met in the data path

>The arrival time is equal to the Tcq + Tcombi, and the Required time is equal to the Tclk – Tsu

> The timing in the path will be violated if the arrival time is more than the required time, slack = required time – arrival time, if slack is negative, then the timing is violated

![](https://github.com/YishenKuma/sd_training/blob/main/day8/25.jpg)

> now we are reporting our timing once we have told the tool the clock uncertainties to take into consideration, our slack has decreased as the clock uncertainty introduced has been removed from our data required time, making our slack reduced as well. The skew introduced will look to not help the setup and hold, as to act for pessimistic timing. Our data required time is equal to Tclk -Tsu – Tuncert. 

> Setup timing is a 1 cycle check, launch is at zero, capture is at one. For setup timing, the data reaching the capture pin will be pulled back due to the uncertainty, skew is reducing the available window for setup, Tclk - Tsu – Tuncert must be higher than Tcq + Tcombi. If we cannot set a value for uncertainty such that the arrival time becomes greater than the required time.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/26.jpg)

> we can see the effect of the clock_uncertainty type min in our report_timing -delay_type min, where the 0.1 introduced is assed to our data required time, instead of subtracted. For hold timing,   the data arrival time needs to be more than the data required time. So our slack will be decreased with the hold uncertainty introduced, as the required time becomes higher.

> Hold timing is  a 0 cycle check, as the launch and capture is both at zero cycle. For hold timing, the data reaching the capture pin will be shifted forward due to the uncertainty, the skew will reduce the available window for hold. Our calculation for slack will be met as long as Thold must be less then minimum Tcq + Tcombi. With the introduction of delay, the Thold + Tskew must be less then minimum Tcq + Tcombi.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/27.jpg)

> reports all the ports show us no values for the input transitions and output load, this is because we have not introduced these elements to our design yet

![](https://github.com/YishenKuma/sd_training/blob/main/day8/28.jpg)

> if we look at our timing report from our input port or to our output port, we can see that the path is not yet constrained

#### IO delays

![](https://github.com/YishenKuma/sd_training/blob/main/day8/29.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day8/30.jpg)

> modelling the inputs, outputs for min and max delays, and we will get a constrained path. We need to set both the max and min or else either setup or hold will be unconstrained.

> we can also use the -cap -net, and -trans option for report timing to see the capacitances and transmittance 

Our timing paths still need to factor in the input transitions as well

![](https://github.com/YishenKuma/sd_training/blob/main/day8/31.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day8/32.jpg)

> the input transition will also cause the slack to decrease, the value of period needs to high enough to take into account of the delays introduced or the timing will be violated

![](https://github.com/YishenKuma/sd_training/blob/main/day8/33.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day8/34.jpg)

> setting the output load, the load introduced will cause the delay to get worsen as well and reduce the slack available

#### generated clocks

![](https://github.com/YishenKuma/sd_training/blob/main/day8/36.jpg)

> if we look at our timing report at the moment, we can see there is no difference in the clock network delay for . We need to maintain the IO delay with respect to the clock at the output point, as there may be a routing delay that could happen for the clock at that point, it is best to annotate this separately.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/37.jpg)

> We create the generated clock using command create_generated_clock. We can see this clock using report clocks. We can also see if the attribute for the clock is set true for is_generated.

> However, our timing paths are still shown with respect to the master clock only, we want our capture to be shown with respect to our generated clock. We need to set the constrains on the design through the generated clock.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/38.jpg)

> Now we can see that our timing path has been modelled to take into account the clock latency and output delay, thus our data required time has changed as a result.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/39.jpg)

![](https://github.com/YishenKuma/sd_training/blob/main/day8/40.jpg)

> these commands can be written out in a command script, and then used for a design. We can then check on whether these constrains have been set through the report_ports command.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/41.jpg)

#### set max delay

> Now we will work with a similar circuit with an additional 2 inputs that are fed through an XOR gate and coming out as new output port. Since our design is similar, we can use the same constraint file written earlier. 

![](https://github.com/YishenKuma/sd_training/blob/main/day8/43.jpg)

> As can be seen, the timing path to output Z has not been constrained yet, since this design is having the 2 new input ports and 1 new output port. The timing path from IN_C will also show unconstrained path. 

![](https://github.com/YishenKuma/sd_training/blob/main/day8/44.jpg)

> Now we have set a max delay of 0.1 from all inputs to Output Z, we can no see that the timing path has been constrained. The reason why this path is violated is because ewe have set this constraint after synthesis, so the tool has not yet optimized the path 

![](https://github.com/YishenKuma/sd_training/blob/main/day8/45.JPG)

> Now we can see the timing path has been optimized based on the constraint set, and we are no longer violating. This is because the tool has modified the cells used in the circuit while keeping the same logic, such that the overall combinational delay is reduced to meet the timing requirements. The XOR gate is replaced with a XNOR gate with 1 of the inputs inverted.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/46.JPG)

#### VCLK

![](https://github.com/YishenKuma/sd_training/blob/main/day8/47.JPG)

> now we have created our virtual clock which no sources. 

![](https://github.com/YishenKuma/sd_training/blob/main/day8/48.JPG)

> once we have constrained the path by setting the input and output delays on the ports IN C , IN D and OUT Z. The report timing  will be constrained, however the design is violated because the available time of (10 -5 - 4.9 =0.1) is not sufficient for the combinational logic of 0.12, thus its is violated by 0.02.

![](https://github.com/YishenKuma/sd_training/blob/main/day8/49.JPG)

> Similarly to before, once we perform synthesis with regard to the constraint set, the optimization is performed and the logic is squeezed. Now our timing is met in the timing path.

</details>

## **Day_9 : Optimizations in Synthesis**

<details><summary>  Lecture + VSDIAT recording topics </summary>

Optimization goals are to:

* enable optimization until cost is met 

* control optimization performed, as optimization of one goal will harm other goals, the goals for synthesis is to meet timing, power, and area, and these three metrics are contradictory

#### Combinational Optimization 

Combinational optimizations saves power and reduces area by squeezing logic to get the most optimized design. 

> One method which is used is known as constant propagation or direct optimization. This is the method of substituting  the values of known constants into expressions, and simplifying the logic, and then the hardware implementation can be minimized.

The second method used is Boolean logic optimization (k-map , Quine McKluskey) 

>  Boolean optimization refers to minimizing the Boolean functions . The simplification of the Boolean expression will lead to reduction in cost and complexity of design as the Boolean expression has been simplified. 

We also have resource sharing, in which the cells are shared for usage instead of being used in a manner that may take up more requirement than necessary. The number of operators are reduced and the subsequent logic will be minimized. 

Logic sharing is the process of optimization in which common logic within multiple expressions are shared to wherever it is applicable to reduce usage of complexity of design. 

##### Balanced vs Preferential Implementation

A balanced implementation is when each input will have around the same amount of delay throughout the combinational circuit. A Preferential implementation is when we are having paths that are more tight compared to others,  in this case the implementation can be performed to favour the tighter path with sacrificing on the timing to other paths, meaning adding more gates to the inputs.

#### Sequential Optimization

The basic methods of sequential optimizations are: 

* Sequential Constant Propagation

A constant is a sequential constant if it is able to produce an output that can be simplified compared to the original logic. If the output is unique with the constant, then it is not a sequential constant, and the logic cannot be optimized through this method.

For example, a SET flop with D set to high, will produce an output of high regardless of change in SET or clock, thus the logic is simplified to output = high.

* Retiming

* Unused Flop Removal

* Clock gating

* Optimization of unloaded outputs

There can be cases in which within the written Verilog, there are unloaded outputs, meaning the output of the design may not initialize on all outputs within the design. In this case,  the unused outputs may be optimize out and the circuit may be simplified based on the loaded output.

> example: [unused output optimization]( https://github.com/YishenKuma/sd_training/blob/main/readme.md#unused-output-optimization)

The advanced methods of sequential optimizations are:

* state optimization

* sequential logic cloning (floorplan aware synthesis)

There may be cases however where we may want to retain the logic and not have optimization performed. This can help in the case where we can retain logic in the case that specs need to be changed. We can prevent the optimization from happening and preserve the logic and components to be used if needed. 

The way we can control the sequential optimizations in DC is through the usage of the variables: 

* compile_seqmap_propagate_constants

> setting this as fales will not propagate the sequential constants

* compile_delete_unloaded_sequential_cells

> setting this as fales will not optimize designs where there are unused outputs

* compile_register_replication

> setting this as false will not allow for register cloning to optimize timing on high fanout nets 

#### Special Optimizations

* register retiming

If we have a very complex combinational circuit in path that we want to further optimize, it is not so easy to partition the logic to be optimized. One way we can perform this additional optimization is by adding flops to the outputs, such that we introduce slack on the path, then we can slice a portion of the combinational logic and put it between the flops, that way ,the slack of the flops will be reduced, and the delay of the combinational logic will be delayed. Now that the critical path delay has reduced, our frequency can be increased, this is known as register retiming. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/36.JPG)

In register retiming, we need to keep in mind the larger picture. The disadvantage in doing this is that in dividing the logic, we will have intermediate values after the flops, and these cannot be matched to the rtl waveforms. In the case that this type of optimization does not gel with the overall flow, then it is best to disable this. The repercussion of enabling this would mean that we would not know how the logic is being partitioned. 

* Boundary optimization

![](https://github.com/YishenKuma/sd_training/blob/main/day9/37.JPG)

When we enable boundary optimizations, the tool may dissolve boundaries present for modules in order to combine logic to get an optimum logic, this boundary will not be in the netlist anymore. The disadvantage of this method of optimization is that the functional (DV) design verification may have issues, as the hierarchical level is no longer there, we can longer find the previous signals within the boundary. The option for enabling or disabling boundary optimization is with set set_boundary_optimization <design> true|false.

* Multi-cycle paths

There can be some cases where the data need not be sampled on the first clock cycle. If the data for a path will only be sampled once every 2 cycle paths, then the tool needs to be told this, or else it will try to unnecessarily optimize the path as a single cycle path, the tool may overoptimize on the path and use up resources instead of optimizing on other paths. We can do this using the command set_multicyle_path. 

* False paths

False paths are paths that are not valid for STA. If we are having a path between two cells which are clocked differently, then we can set this path as a false path, since there is no relation between clock 1 and clock 2 .We perform this using the command set_false_path. An important thing to note that path is only async if the 2 clocks are not related, not just different, 2 clocks may be different but they can still be related.

* External load vs Internal load 

Sometimes in our design we can have a internal feedback at the output that is connected to the output load. If we were to increase the output load, then out internal feedback path will also be affected, as the delay would increase due to increase in output load, this is not what we want. To avoid this, we use set_isolate_ports, so that the internal path will not see and be affected by the output load. 

#### How timing is checked?

* single cycle paths

![](https://github.com/YishenKuma/sd_training/blob/main/day9/38.JPG)

For single cycle paths, the capture edge will be on the consequent rising edge of the capture flop, for setup check. For hold timing, the capture edge will be one edge before setup. 

* half-cycle paths

![](https://github.com/YishenKuma/sd_training/blob/main/day9/39.JPG)

For half cycle paths, in which the capture flop clock pin is inverted. The capture edge will be on the consequent fall edge of the capture flop for setup check, and for hold it will be the falling edge one cycle before. 

For half-cycle paths, the setup margin is very tight, whereas the hold margin is relaxed. 

* multi cycle paths

![](https://github.com/YishenKuma/sd_training/blob/main/day9/40.JPG)

For multi-cycle paths, where data is getting loaded once in every 2 or more cycles. We need to apply the command set_multicycle_path with the option -setup <number of cycles>. The hold will also be shifted, as the hold check will be checked one cycle before setup. However, this will cause the hold to be violated

![](https://github.com/YishenKuma/sd_training/blob/main/day9/41.JPG)

The way to handle is to run an additional set_multicycle_paths command but with the -hold < number of cycles - 1>. This will make it such that the launch edge is now shifted forward.  

</details>
	
<details><summary> Lab day 9 </summary>
	
#### Combinational Optimization 

##### opt_check1

![](https://github.com/YishenKuma/sd_training/blob/main/day9/1.JPG)

>  from this Verilog file, we can see that there are 2 outputs, and for the two outputs, we constants used at the input points. 

> For y1, the mux is selected between 0 and b based on the value of a. the logic will be y1 = !a.0 + a.b , which results to y1 = a.b. 

> for y2, b is fed into and agte with constant 0, so resulting output will be 0, then this is fed into or gate with c, and the output is fed through inverter. Our final output will be y2 = !(c + (0.b) ) = !(c + 0) = !c.

Thus through constant propagation, we will reduce the logic to the use of 1 and gate and 1 inverter.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/2.JPG)

> as can be seen, after the compile is performed, the design is show the 2 components as discussed above. 

##### opt_check2

![](https://github.com/YishenKuma/sd_training/blob/main/day9/3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/4.JPG)

> for this design, our output, y = a.1 + !a.b = a + !a.b = a + b. The design will be optimized to have only an or gate. 

##### opt_check3

![](https://github.com/YishenKuma/sd_training/blob/main/day9/5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/6.JPG)

> for this design, our output, y = a.[c.b + !c.0] + !a.0 = a.c.b +a.0 +0 = a.c.b. The design will be optimized to have only a 3 input and gate. 

##### opt_check4

![](https://github.com/YishenKuma/sd_training/blob/main/day9/7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/8.JPG)

> for this design, our output, y = !a.!c + a.((!b.a.c) + (b.c)) = !a.!c + a.!b.c +a.b.c = !a.!c +a.c. The design will be optimized to have only an xnor gate. Input b will be unused.

#### Resource Sharing Optimization 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/9.JPG)

> Based on the logic written in the netlist, the out put y will either be the result of a.b or c.d based on the value of sel, which would mean a use of 1 mux and 2 and gates, however as we discussed previously, through resource sharing, the logic can be optimized to use only 1 and gate with 2 muxes instead, which is better for power and area.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/10.JPG)

> through the command report_area, we can see the area taken up by the combinational circuit as well as the list of devices used in the design. For this case, we have an area of 455.43, 42 ports, and total of 127 cells used. The mux is located at the start of the beginning of the logic, and not toward the output. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/12.JPG)

>we can see that the design is broken into 2 parts, wherein the left side where the inputs are, the select lines are initialized into multiple muxes for each of the inputs a, b, c and d. Then on the right side we have the multiplier circuit. This is how the resource sharing is done, instead of having the mux closer to the outputs, the mux goes through many more combinational gates. 

> we have set a max delay of 2.5 from all inputs to all outputs and synthesized the design. But what would happen if we made the timing path for select more restrictive.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/13.JPG)

> after we set the max delay from sel to all outputs at value of 0.1, our timing is much more restrictive and out timing path is now violated.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/14.JPG)

> now we perform synthesis once again and the design has been optimized based on the dependency of the restrictive path. We can see that our design has been greatly altered. The area and number of cells has increase greatly, this is because the optimization is done with regard to the restrictive path of sel, the timing needs to be ensured there, so the number of gates from that path is minimized while sacrificing on other paths.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/15.JPG)

> select is not being used by the inputs, and instead is used directly to the outputs. This way the number of gates the sel path passes through is reduced and the timing can be met.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/16.JPG)

> timing is met for  the restrictive path

![](https://github.com/YishenKuma/sd_training/blob/main/day9/17.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/18.JPG)

> now we are going to restrict the design by setting a maximum value for area, previously after the previous synthesis, the previous area was above 900, now we will set a max value of 800. We can see that our timing is met and the are has been reduced below the max value. The number of cells and area have reduced, but the area was not able to be lower than the max value set, this may be due to the highly restrictive timing path.

#### Sequential Optimization

* dff_const1.v

![](https://github.com/YishenKuma/sd_training/blob/main/day9/19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/32.JPG)

> the Verilog file states that the asynchronous flop will output low upon high reset, and high for low reset.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/24.JPG)

> we can see the cells of the design, a flop, inverter and a conb cell has been inferred. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/25.JPG)

> The input d has been connected to the logic 1 pin of the conbi cell, which is a tie cell. In propagation of Vdd through design for all the components, there can be transience in the power that happen due to current being drawn from cells, this transience in the power cannot be seen by the gate terminal of CMOS, as it is very sensitive, therefor the D pin of sequential elements should never connect directly to the Vdd pins, but instead be connected to tie cells which can produce the 1 or 0 signal without any transience.  

* dff_const2.v

![](https://github.com/YishenKuma/sd_training/blob/main/day9/20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/33.JPG)

> for this Verilog code, the asynchronous flop will output high upon high reset, and high for low reset.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/26.JPG)

> our design is now only showing the q pin connected directly to the tie cell, the reason for this is as mentioned before, the design is optimized due to the sequential constant that will result in an output of 1 regardless of change in clk and reset pin. 

* dff_const3.v

![](https://github.com/YishenKuma/sd_training/blob/main/day9/21.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/34.JPG)

> here we have 2 asynchronous flops, where the first flop is a reset flop and the second flop is a set flop. The output of the first flop is connected to the input of second flop. In this logic, the output of our first flop will low from any point which the reset signal rises, until the clock rising edge after reset goes low. For the second flop however, during the period of set being high, the output will be high, and once the set goes low, the output will be set to the value of q1, which will should be high, however, we need to take into account the delay during that rising clock edge between flop 1 and flop 2, flop 2 will capture 0 before q1 has gone high, and q will only go high during the next rising edge. So q will is not be always high, and the design cannot be optimized based on this. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/27.JPG)

* dff_const4.v

![](https://github.com/YishenKuma/sd_training/blob/main/day9/22.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/35.JPG)

> in this case, both asynchronous flops are set flops, instead of previously where one was a reset flop. In this case, the flop behaviour is the same as from the dff_const2 design, so the output q should be always high. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/29.JPG)

> the design has been optimized.

* dff_const5.v

![](https://github.com/YishenKuma/sd_training/blob/main/day9/23.JPG)

> in this case, both flops are reset flops, so the waveforms would most likely be as follows. This design would not be able to be optimized. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/30.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/31.JPG)

* Using option compile_seqmap_propagate_constants

![](https://github.com/YishenKuma/sd_training/blob/main/day9/28.JPG)

> lets take dff_const 2 which was able to be optimized earlier through sequential optimization. If we set the option compile_seqmap_propagate_constants to false, the the optimization should not be possible. As we can see form the above schematic, the sequential constant has not been propagated and the design was not optimized. 

#### Boundary Optimization 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/42.JPG)

> in this code, we are having an internal module, which contains the logic for a counter, which outputs data to the external top level when the value is ‘111’. This output is then connected as the enable pin for the mux connected to the input of flop in the top level. The asynchronous flop input is muxed between val_in or the feedback of output. 
 
![](https://github.com/YishenKuma/sd_training/blob/main/day9/43.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/44.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/45.JPG)

> if we set the option set_boundary_optimization to false, then no optimization will be not be performed and the internal module and logic will remain the same.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/46.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/47.JPG)

> Now we set the boundary optimization true for u_uim. We can see that the internal module is no longer there. The pins for u_im and u_im cell no longer exist as well as optimization has combined the logic with the top level logic.  

#### Register Retiming

![](https://github.com/YishenKuma/sd_training/blob/main/day9/48.JPG)

> in this Verilog file, we are having a multiplier followed by three registers between ports a, b, and c. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/49.JPG)

> we can see the multiplier circuit as an internal module, connected to the top level 3 registers.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/50.JPG)

> now that we have constrained the path, we can see that our timing path from the input path is violated

![](https://github.com/YishenKuma/sd_training/blob/main/day9/51.JPG)

> using the command, compile_ultra -retime, our design has now changed. Now we can see that the multiplier circuit has been sliced and put in between the registers. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/52.JPG)

> the timing path is still violated but now it is reduced

#### Isolating output ports

![](https://github.com/YishenKuma/sd_training/blob/main/day9/42.JPG)

> using the similar code from earlier, there is a feedback path that is providing the input feedback if enable signal to mux is low. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/53.JPG)

> we can see the feedback path in the design above. We can see that the output port is driven by the same internal logic, which is undesirable, as the more the output load varies, the more the internal path will get affected. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/54.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/55.JPG)

> Now we set an output load on the design, we can see this load being reflected onto the reg to reg paths. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/56.JPG)

> The way we solve this is by isolating the port using command set_isolate_ports on the output port. Now we can see from the design after we optimize, the internal paths are isolated from the output port and any possible external load. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/57.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/58.JPG)

> the timing report for the reg to reg path will also reflect this change, as the load is no longer effecting the path.

#### Multicycle Paths

![](https://github.com/YishenKuma/sd_training/blob/main/day9/59.JPG)

> in this verilog, we have 2 registers, where the output of the first register is connected to the enable pin of a mux, connected to the input of the second register. The mux output will be a.b only if the output of the first register is high. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/60.JPG)

> if we set our constraints and report timing, we can see that the timing path is greatly violated. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/61.JPG)

> now notice how the timing path is still violating after the compile_ultra command has been run. This is because in our design the output of register 1 will take a half-cycle before a high can be captured, this means that, our second register will only capture data at the second clock cycle. Thus we need to set this path as a multicycle path. Be sure to specify which paths to be set as multicycle paths, and not affect the single cycle paths. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/62.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day9/63.JPG)

> once we have set our multicycle path, we can see that our timing path is no longer violated. If we look at the the timing path from all inputs, we can see the capture is happening at 8ps, instead of at 4ps.

![](https://github.com/YishenKuma/sd_training/blob/main/day9/64.JPG)

> however, if we look at the hold check, it is still violated, this is because the capture edge for the hold check has been shifted to the right as well, meaning the launc is at 0ps while capture is at 4ps, which is not good for hold check, as it is not a single cycle check. To solve this, we need to set_multicycle_path again for -hold. 

![](https://github.com/YishenKuma/sd_training/blob/main/day9/65.JPG)

> as can be seen, the path is no longer violating, and this is because the capture edge has been shifted backward to 0ps instead of 4ps. 

</details>

 ## Day_10 : QOR**

<details><summary>  ### Lecture + VSDIAT recording topics  </summary>

#### Report Timing Generation and Analysis

One thing to understand for timing paths within a logic circuit is that the propagation delay is not the same between the timing paths,  (Input[rise] to Output[fall]) and (Input[fall] to Output[rise]). The reason for this is due to the fact that the mobility of holes is not equal to the mobility of electrons. Different input logics will have different input transitions due to difference in charge in the combinational logic, as such rise time and fall time will not be the same.

The usage of the option “-delay_type min” when using report timing shows the timing path from the startpoint at the fall edge. Default setting for timing report is to show -delay_type max, which is to show the timing path from startpoint at rise edge.  These timing paths will not be same as mentioned before, the fall and rise time for components are not the same. 

The usage of the option -fall_from/rise_to when using report timing will show the timing path of which the specified edge of specified pin is either fall edge or rise edge.

For setup, he arrival time refers to the time taken for the data to go from the input through the gates to the output endpoint. The required time will be the clock period minus of the setup time and delays introduced on the circuit. The setup slack will be the required time – the arrival time. 

For hold however, as it is a zero cycle check, there will be no period on the required time, so it is only the hold time and the uncertainties. The hold slack will be equal to the arrival time – the required time, as data should change only after data hold time. 

The timing path report is run without options will show the timing path with the lowest slack, if any of the paths has a negative slack, meaning it is violating, then that path will be shown.

</details>
	
<details><summary> Lab day 10  </summary>

#### Report Timing

![](https://github.com/YishenKuma/sd_training/blob/main/day10/1.JPG)

> Verilog file used for lab, in which 3 flops are used with combinational logics are used between the flops.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/2.JPG)

> Once the constraints on the design have been set, and design is compiled, we report the timing. The ways we can tell that this is a setup check is from the path type, which is max. and the launch edge is at 0 while capture edge is the next cycle. There is also a library setup time shown. The slack is calculated based on required time – arrival time.

> the option -from IN_A. The path assumes a fall from IN_A. The letter after the time taken through path f/r denotes either fall or rise. The fall to rise time of U14 is 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/3.JPG)

> by default, this is the worst timing path seen by design, if we use the option -rise_from IN_A, we will see the timing path assuming rise edge from IN_A. Notice how the delay is different compared to the delay in fall edge previously.  The rise to fall time of U14 is . The slack is calculated based on arrival time – required time.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/4.JPG)

With the option -delay min, we are now checking the hold timing path. Notice how the capture and launch are at the same cycle path. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/5.JPG)

> we can also use the -thr option to see the worst timing path that passes through specified pin. This is by default the max timing path.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/6.JPG)

> notice between the setup and hold path through U15/Y, the cell is taking a delay of 53 ps in the max path while taking a delay of 66 ps. The reason for this is because even though we set the timing path to be max, the delay through the cell may not necessarily be at its max delay, as the max option for timing path is dependant on the overall delay. 

#### Check Timing, Check Design, Set max capacitance, HFN

There can be problems in loading the design into the tool due to human error that might have been overlooked. In order to check whether the loaded was correctly loaded into the tool, there are a few commands that can be used to verify if design loaded correctly. 

* check_design 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/7.JPG)

> check_design shows there is a feedthrough from the input port clk to the output port clock, which is perfectly fine.

* check_timing

![](https://github.com/YishenKuma/sd_training/blob/main/day10/8.JPG)

> check timing will check whether the design is properly constrained or not, since we have not set any constraints on the design, it is not proper, and thus the check is showing warning. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/10.JPG)

> once we set these constraints, these warnings prompt will no longer appear, excluding for the clock points, as we can constrain a data port with a clock port, but not a clock port with itself, so the clock ports do not be defined, so these warnings are not significant.  

* report_constraints

![](https://github.com/YishenKuma/sd_training/blob/main/day10/9.JPG)

> report will show only the tool default constraints from memory if no constraints are defined on the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/12.JPG)

> once constraints, have been defined, the report will show these constraints. The report will also show the max transition, max capacitance, max delay/setup, etc.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/13.JPG)

> this verilog file is for a 127 – 1 MUX, in which the y will be assigned to the value of input k if the value of sel is equal to k during the for loop for 128 iterations. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/14.JPG)

> If we synthesize this design, there will be no sequential cells, as y was assigned in a for loop within always, the latch was inferred during read_verilog due to the always statement. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/15.JPG)

> the select is going to so many fanout nets, we need to filter this as the higher number of fanouts will increase the capacitance of the net. Our timing path will be violated greatly as a result. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/16.JPG)

> report_constraint -all_violators will show all the violating paths.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/17.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day10/18.JPG)

> now we perform compile ultra with max delay and max capacitance values set. Now we can see that everything has been met (leakage power is negligible). Our timing path will also be optimized to not be violated as well.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/19.JPG)

> our net capacitances have also been reduced compared to previously, this is because the high fanout nets have been broken up to lesser fanouts. Whenever we perform synthesis,  we should limit the capacitance so that high fanout nets can be buffered early. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/20.JPG)

> This verilog file had 128 output pins being used by the design, compared to previously where only 1 output pin is used for 1 value of y assigned to k. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/21.JPG)

> we can see our net is having a fanout of 128, which is causing an extremely high capacitance value. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/22.JPG)

> once we set the max capacitance value, and perform synthesis, the high fanout nets will be broken, and the capacitance values will be reduced and met within constrained value. Instead of 1 net faning out into 128 nets, it will break into a small number of nets, which will further break into more nets sequentially. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/23.JPG)

> the high fanout net is split such that the single pin is not having the burden of driving such a heavily loaded net. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/24.JPG)

> Our trans value is still quite high however, the way we offset this in synthesis is by setting max transition.

![](https://github.com/YishenKuma/sd_training/blob/main/day10/25.JPG)

> the paths which are having transitions violated. 

![](https://github.com/YishenKuma/sd_training/blob/main/day10/26.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day10/27.JPG)

> once we synthesize design with constrained transition, there will no longer be any violating paths. The synthesis tool has changed the buffer to have a higher drive strength to be able to meet the max trans value of the design.

</details>
	
## **Day_11 : Introduction to BabySOC**

<details><summary> Lecture 11 </summary> 
	
### What is SoC and Why SoC?

![](https://github.com/YishenKuma/sd_training/blob/main/day11/1.JPG)

SOC stands for system on chip.  It is a single-die chip that integrates different IP cores on it. These IPs can vary from digital uses (microprocessors) to analog uses (5Gbroadbandmodems)
 
The SOC design usually includes the CPU, memory interfaces, memory interfaces, on-chip input/output devices, input/output interfaces, and secondary storage interfaces, often alongside other components such as radio modems and a graphics processing unit (GPU), all on a single substrate.

The design of SOC can also vary depending on the requirement, to consist of either digital or analog signal processing system or floating-point unit.

The functionality of an SOC is based on its performance, power consumption, and semiconductor die area. A greatly designed SOC will have higher performance while having reduced power consumption on a small area. 

### Typical structure of Snapdragon SoC

![](https://github.com/YishenKuma/sd_training/blob/main/day11/2.JPG)

The snapdragon SoC’s are a type of SoC designed for mobile devices. The SoC acts as the brains of the phones which handles everything from the operating system to user inputs. The SoC design incorporates different modules to allow the various uses of a mobile device such as the Wifi, GPS, Camera, Media storages, Display, etc.

### Types of SoC

We can have SoC either built a microprocessor, microcontroller, or built as a specialized application-specific IC SoC for specific applications no suited for the microprocessors and microcontrollers. 

### SoC Structure

![](https://github.com/YishenKuma/sd_training/blob/main/day11/3.JPG)

The SoC design structure consists of hardware functional units, including microprocessors running software code, as well as communication subsystem needed to connect, control, direct, and interface between the functional modules. The intermodule communication of an SoC design includes bus-based communication and network on chip.

The Functional components examples:

* processer cores: refers to the brain if the CPU, retrieving instructions and performing operation and calculations based on the instructions

* memory: RAM/ROM, needed for storing huge datas

* DSP: digital signal processor, used ofor audio signal and digital image processing, as well as telecommunications and sonar and radar 

* Encoder/Decoder: combinational circuitry used to modify wither binary data into a number of output lines, or a number of output lines into binary data, fundamental in translation software

* Network Interface card: provides device with full time connection to network 

* GPU: Graphical processing unit, designed to handle graphics such as 2d and 3d, and video more efficiently.

* Peripheral devices: provide the input/output functions for computer, does not perform any core somputing process but simply allows connection between computer and external devices to allow more capabilities and functionality

* UART : Universal Asynchronous Receiver Transmitter, a universal serial communication protocol that transmits data serially between systems, can be used for both transimission and reception


### SoC Design Flow

![](https://github.com/YishenKuma/sd_training/blob/main/day11/4.JPG)

The design flow of an SoC starts at design specification, which is the most crucial step where the specifications of the system are defined and created. 

Architecture design where the blocks to be used are decided and the hierarchy system is chosen based on the operating system to meet the design specifications. 

The logic design/schematic design has to be made for the system to realize the design during the basic logic design.

Then the logic of the system will need to be verified, to establish if the system functionality is as intended. If the logic is not as intended then, modification would be needed. 

Following this, the design would be translated from a schematic level to a physical level using basic building blocks.

Then similarly, we need to verify the physicality of layout based a few important checks which are DRC (design rule checks), LVS (layout versus schematic), power and timing analysis. 

Once the design is verified and the GDS file has been created, it is appropriate to proceed for the fabrication of the design.

### How are Microchips made?

![](https://github.com/YishenKuma/sd_training/blob/main/day11/5.JPG)

The flow of fabrication begins with the slicing of silicon ingots into wafers, which are polished and cleaned. Then we will begin epitaxial growth, which is the process of growing the layer of silicon dioxide onto the surface of wafer.

The two main steps in transferring the complex design of an SoC is through Photolithography and etching. 

Photolithography is the process of making the wafer with a layer of light-sensitive liquid uniformly, and then exposing the pattern of the design on to the wafer, shot by shot, causing the exposed areas to become hardened, and areas that were not exposed can be washed away, leaving only a mask of the design.

The etching process is to remove the wafer surface to create the necessary patterns of the design based on the mask created in the photolithography stage. Either through chemical or physical etching, the substate is etched away to leave the necessary holes for other steps in the flow such as doping or metallization. 

Doping is to create the necessary n-wells and p-wells by altering the properties of the silicon through doping with elements such as boron or phosphorus. 

Metallization is where a thin layer of aluminium will be deposited to create the necessary connectivity of the design. 

These steps will be repeated again and again for each successive layer until al the chips are complete.  

### Introduction to BabySogC

![](https://github.com/YishenKuma/sd_training/blob/main/day11/6.JPG)

 BabySoC refers to a small chip but a powerful RISC V SoC, the main purpose in designing this is to test 3 open source IP cores and calibrate the analog component of the design. The baby SoC contains an PLL to generate stable clock, and a 10 bit digital to analog converter to communicate with other analog devices. The babySoC also contains an rvmyth processor which is simple RISC V based CPU. 

* RISC V

RISC V is an open standard instruction set architecture (ISA) based on established RISC principles. RISC V is used by many developers because it simplifies the instructions given to the processors to accomplish tasks, as well as provides the flexibility to create thousands of possible custom processors. This allows companies to get their designs marketed faster. 
RISC V applications include artificial intelligence, augmented reality, automotive, cloud srevers, computing decides and controllers, general purpose processors, internet of things, machine learning, network edge, and virtual reality.

### BabySoC Components

* RVMYTH

Refers to the core, which is a simple RISC V based CPU

* PLL

PLL stands for phased locked loop, which is a control system that generates an output signal with a phase related to the phase of the input signal. PLL are used for synchronization purposes, including clock generation and distribution.

* DAC 

DAC stands for digital to analog converter, it is a system that converts digital signal into an analog signal. DACs are widely used in modern communication systems for the generation of digitally defined transmission signals.

### Introduction to Modelling

The modelling refers to the integration of the components together to create the babySoC.
Some initial inputs will be fed into the design to make the PLL start generating the proper clock for the circuit. Then the clock signal will make the processor start executing instructions in its imem. Then the register will be filled with a value each cycle. These values will be used by dac core to provide the final output. 

</details>
	
 ## **Day_12: BabySoC Modelling **

<details><summary> ### Lecture Day 12 </summary>

#### Modelling and simulation

Modelling and simulation refers to using a logical or physical representation of a system to generate data and help make decisions or predictions on a system.

Models are representations that can help to define, analyse and communicate a set of concepts to user. System model also support specification, design, verification, and validation of system.

For our design on the babysoc module, we will have some initial input signals be fed into, which will get the pll to start generating the proper clock for the circuit. The clock signal will get the core rvmyth to execute instructions and generate values, these values will then be used by the DAC to provide the final output signal. So in total we have 3 main elements, the core, pll, and the DAC, alongside a wrapper as an SoC with the corresponding testbench module. 

* RVMTYH core

RVMYTH is a Risc V based MYTH (Microprocessor for You in Thirty Hours). RISC (Reduced Instruction Set Computer) ISA is defined as a base integer ISA, which must be present in any implementation, plus optional extensions to the base ISA. RISC V is very popular in industry standard due to its ability to expand the instruction set based on any processes your chip will need for a given product. 

Each base integer instruction set is characterized by the width of the integer registers and the corresponding size of the address space and by the number of integer registers. The base is carefully restricted to a minimal set of instructions sufficient to provide a reasonable target for compilers, assemblers, linkers, and operating systems (with additional supervisor-level operations), and so provides a convenient ISA and software toolchain “skeleton” around which more customized processor ISAs can be built. 

> https://riscv.org/wp-content/uploads/2017/05/riscv-spec-v2.2.pdf

![](https://github.com/YishenKuma/sd_training/blob/main/day12/1.JPG)

This is a diagram for a simple one-cycle CPU for Risc V. We have the program counter,  the decoder, memory elements, resistor file read and write, Arithemtic Logic Unit. 

![](https://github.com/YishenKuma/sd_training/blob/main/day12/2.JPG)

The flow starts with the program counter, then the data is fetched and then decoded, after that the memory is read, and then the code is executed, finally the output is written. Parallelly next line will go through the program counter, while the previous line is being fetched. This happens continuously to allow better time optimization. There are also pipeline hazards that need to be accounted for during the flow. 

* PLL

Phase locked loop is an electronic circuit with a voltage or voltage-driven oscillator that adjusts continuously to match the frequency of an input signal. Some uses of the PLLs are to generate, stabilize, modulate and demodulate. 

The reason why we need PLL for SoC designs of frequencies above 100Mhz is because when we are having large designs with longer routings, the design is subject to clock jitter due to the delays from the long routing. PLL allows designer to set bandwidth to an appropriate value to balance the need for jitter filtering. 

Within the design itself, we can be having different frequencies, which we cannot achieve with off-chip clocks. 

The clock accuracy is dependant on the ppm error (parts per million) of the clock, which indicates how much our clock crystal frequency may deviate from the nominal value. 

![](https://github.com/YishenKuma/sd_training/blob/main/day12/4.JPG)

> https://www.sharetechnote.com/html/Electronics_PLL.html

The components of a PLL includes a phase detector, a loop filter, a voltage controlled oscillator and a frequency divider. 

![](https://github.com/YishenKuma/sd_training/blob/main/day12/3.JPG)

The frequency divider is necessary to produce an output that is a division of the clock input by a certain factor. This allows us to use different frequencies in our design. 

* DAC

Digital to analog converter translates the digital input signal, represented by binary code,  into an analog output signal. However, this design is very limited as the larger the resistor that needs to be used, the more heat will be generated by design

![](https://github.com/YishenKuma/sd_training/blob/main/day12/5.JPG)

This can be done using weighed resistor DAC, which performs the translation using binary weighted resistors in the inverting adder circuit. 

![](https://github.com/YishenKuma/sd_training/blob/main/day12/6.JPG)

Another approach to this would be using the R-2R ladder,  which overcomes the issue previously as the number of resistors required to realize the design will be much fewer in comparison. We only need 1R and 2R pair for each bit of resolution.

#### Modelling BabySoC

One thing to take not that verilog cannot synthesize analog designs, and PLL and DAC components are both analog designs. How we overcome this is by simulating them using verilog itself. We will focus on the functionality of the components instead of modelling it first. We will be using real data types in our designs for these components. Real data types are not synthesizable, but they can be used in simulation. 

The goal is to ensure the functionality of the design by verifying the logical correctness through the simulation. 

We will be using verilog to model, and the tool that will be used is VCS. VCS is a high-performance, high-capacity Verilog simulator that incorporates advanced, high-level abstraction verification technologies into a single open native platform.

Modelling and simulating involves 2 steps, Compilation and simulation. During compilation, VCS will build the instance hierarchy and generate a binary executable simv. This binary executable is later used for simulation. Simulation is running the simv file. 

We can either use the tool normally or through interactive mode, which allows debugging for the designer. In the debug mode, we can modify the code and view the changes in the simulation directly. The tool used to view the simulation is DVE (discovery Visualization Environment). 

 Few tips to be awae of in modelling design are:

> Avoid using race conditions

> use an optimized testbench for debugging

> create models that simulate faster

> beware of if-else usage as it is priority dependant, case statement behaviour may be more useful for the design

</details>

<details><summary> Lab Day 12 </summary>

Compile the design using the command “vcs <verilog.v> <testbench.v>”

In the case where the design has real elements, compile the design using the command “vcs -sverilog <verilog.v> <testbench.v>”

“./simv” command will perform the simulation

Then we can view the generated vcd file using “dve &” command

![](https://github.com/YishenKuma/sd_training/blob/main/day12/100.JPG)

> cloning necessary files from github

#### Modelling RVMYTH Core

![](https://github.com/YishenKuma/sd_training/blob/main/day12/101.JPG)

> during compilation of this design, an error encountered due to illegal timescale for the module

![](https://github.com/YishenKuma/sd_training/blob/main/day12/102.JPG)

> looking at the verilog and testbench files, we see the timescale declared in the testbench file, but not in the verilog file.

![](https://github.com/YishenKuma/sd_training/blob/main/day12/103.JPG)

> we solve error by declaring the timescale in both the files

![](https://github.com/YishenKuma/sd_training/blob/main/day12/104.JPG)

> now the design can be compiled with no issue

![](https://github.com/YishenKuma/sd_training/blob/main/day12/105.JPG)

> Our simulation is performed and now we can view our generated vcd file

![](https://github.com/YishenKuma/sd_training/blob/main/day12/106.JPG)

> accessing dve tool

![](https://github.com/YishenKuma/sd_training/blob/main/day12/107.JPG)

> loading vcd file into tool

![](https://github.com/YishenKuma/sd_training/blob/main/day12/108.JPG)

> Now we can see the waveform of our circuit. This design will produce an output of 10 bits that will later be fed into the DAC. 

#### Modelling DAC

![](https://github.com/YishenKuma/sd_training/blob/main/day12/109.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/110.JPG)

> now we run into issues in  trying to compile this design, this is mainly due to the real components of the design. The input of the design is a 10 bit input, and our output will be an analog output. Our input D will change every 10ns, and at each change, the output value will be a computation value of the VREFH and VREFL values set, so output will change around this range each time the input changes. 

#### Modelling PLL

![](https://github.com/YishenKuma/sd_training/blob/main/day12/111.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/112.JPG)

> The Reference signal is the input for the design, which is fed into a phase detector. There is also a signal from the voltage signal oscillator which is fed into the phase detector. The output from the phase detector is passed to the loop filter and then filtered signal is applied to the voltage controlled oscillator. 

> The Voltage Controlled Oscillator, VCO, within the PLL produces a signal which enters the phase detector. Here the phase of the signals from the VCO and the incoming reference signal are compared and a resulting difference or error voltage is produced. This corresponds to the phase difference between the two signals.

> The error signal from the phase detector passes through a low pass filter which governs many of the properties of the loop and removes any high frequency elements on the signal. Once through the filter the error signal is applied to the control terminal of the VCO as its tuning voltage. The sense of any change in this voltage is such that it tries to reduce the phase difference and hence the frequency between the two signals. Initially the loop will be out of lock, and the error voltage will pull the frequency of the VCO towards that of the reference, until it cannot reduce the error any further and the loop is locked.

> https://www.electronics-notes.com/articles/radio/pll-phase-locked-loop/tutorial-primer-basics.php

#### Integration of rvmyth and pll

![](https://github.com/YishenKuma/sd_training/blob/main/day12/113.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/114.JPG)

> we initialize on the previous modules, calling on them to integrate for their functionality. The verilog block for the PLL is first generated, and the output of the PLL is given as an input to the rvmyth. This will create the interface for the place and route to be implemented. 

#### Integration of rvmyth and DAC

![](https://github.com/YishenKuma/sd_training/blob/main/day12/115.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/116.JPG)

> first the verilog module for rvmyth is generated, then the 10 bit digital output of rvmyth will be given to the 10-bit DAC by creating an interface between the two analog and digital blocks.

#### Integration of rvmyth , PLL and DAC all together

![](https://github.com/YishenKuma/sd_training/blob/main/day12/117.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/118.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day12/119.JPG)

> Now we initialize all three modules previously to create the babysoc. Initial inputs are fed into the module to get the pll to start generating the proper clock for the circuit. Then the clock signal will make the rvmyth core start executing instructions within its imem. As a result, the output register will be filled with a value cycle by cycle. These values will then be used by the dac to provide the final output signal. 

> code was modified to allow compilation to be able to execute. Renaming of modules to bring in the correct inputs. Real elements not declared with wire. Timescale declared in both files. And other changes made until no warnings were seen. 

#### Simple Circuit Modelling
 
circuit chosen to be done is the half adder circuity, which is a simple and + or gate combination.
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/11.JPG)
 
> circuit design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/12.JPG)
 
> truth table for circuit
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/7.JPG)
 
> code for half adder verilog, take note to inlcude the timescale in both files
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/8.JPG)
 
> testbench for half adder circuit, be sure to include dumpvars to generate vcd to be viewed
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/9.JPG)
 
> compiling deisgn for half adder circuit
 
![](https://github.com/YishenKuma/sd_training/blob/main/day12/10.JPG)
 
> waveform for design supports truth table, not all states shown however

</details>
	
## **Day_13: Post Synthesis Simulation**

<details><summary> Lecture Day 13 </summary>

#### Pre synthesis Simulations vs Post synthesis simulation

The reason to having pre synthesis simulations, also known as behavioural simulation, is to model the design and check its functionality internally. 

In post synthesis simulation, the entire design is simulated based on the synthesized netlist with respect to the corresponding library files for the design. 

The purpose in the pre synthesis simulation is to check the simulation based on the logic that was designed. Whereas for post synthesis simulation, it is based on the gate delays in the design, which can affect both the timing and functionality. The mismatch between the pre and post synthesis simulation shows what may have been swrongly used for the operators and inference of latches. 

![](https://github.com/YishenKuma/sd_training/blob/main/day13/101.JPG)

The constructs used in the verilog scripts may not be synthesizable constructs, so in performing both pre and post synthesis simulation, there are differences that need to be accounted for in the verilog or testbench files.

#### GLS

Refers to gate level simulation, which is what post synthesis is, where the gate level refers to the netlist view of a circuit. 

The netlist is not just of the gates, but a complete connection list consisting of gates and IP models with full functional and timing behaviours. 

RTL simulation or pre synthesis simulation does not take into account any delay as the events generally occur on the active edge of the clock. GLS however can take into account the timing delays of the library components. 

The purpose of having GLS is to boost the confidence of the design implementation and help verify dynamic circuit behaviour, which cant be done by static methods. 

</details>
	
<details><summary> Lab Day 13 </summary>

We will once again be using DC shell to synthesize the RTL code and then generating the output netlist to be used for the gate level simulation. 

![](https://github.com/YishenKuma/sd_training/blob/main/day13/2.JPG)

> Firstly we need to read in the correct library file, BUT the files must be in .db format and not .lib format, so for this we must convert the /libs to .dbs though the lc shell tool. 

![](https://github.com/YishenKuma/sd_training/blob/main/day13/7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day13/8.JPG)

> Be sure to set the target libraries and the link library for the dc shell pointed to the .db files
 
#### Compiling Rvmyth_asvddac

![](https://github.com/YishenKuma/sd_training/blob/main/day13/9.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day13/10.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day13/11.JPG)

> Keep in mind the non-synthesizable constructs that were mentioned earlier, as real declarations are not supported by synthesis tool, so these elements must be modified from the files. 

![](https://github.com/YishenKuma/sd_training/blob/main/day13/14.JPG)

> the verilog files will need to be error free in order to be able to be read into the tool and synthesized during read_verilog.

![](https://github.com/YishenKuma/sd_training/blob/main/day13/20.JPG)

> Our current design however is not read correctly as the current design is clk_gate.

![](https://github.com/YishenKuma/sd_training/blob/main/day13/21.JPG)

> We need to use the command “read_file {rvmyth_avsddac.v avsddac.v mythcore_test.v clk_gate.v} -autoread -format verilog -top rvmyth_avsddac” in order to set the top module of the design to be rvmyth_avsddac

![](https://github.com/YishenKuma/sd_training/blob/main/day13/31.JPG)

> Linking design

![](https://github.com/YishenKuma/sd_training/blob/main/day13/32.JPG)

> Compiling design

![](https://github.com/YishenKuma/sd_training/blob/main/day13/33.JPG)

> then we generate the gate level netlist to be used for post synthesis simulation using write_verilog

![](https://github.com/YishenKuma/sd_training/blob/main/day13/35.JPG)

> generated netlist

![](https://github.com/YishenKuma/sd_training/blob/main/day13/26.JPG)

> gate level netlist
 
##### Checking design
 
keep in mind we have yet to set any constraints on the design, and any constraint that may be present in loaded from the DC tool memory.
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/36.JPG)
 
>  check_design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/37.JPG)
 
> check_timing

####  Compiling Rvmyth_asvdpll
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/3.JPG)
 
> error in read_lib for asvdpll.lib 
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/4a.JPG)
 
> fixes to file to make it readable
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/40.JPG)
 
> error encountered in reading verilog file due to the real elements that are not synthesizable
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/41.JPG)
 
> real need to be changed to wire, $realtime variable cannot be used and must be replaced with $ytime as realtime will return a value of 1.6, where as what we need is an integer value, which can be reuturened by using $time instead. 
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/42.JPG)
 
> reading in design after appropriate changes made
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/43.JPG)
 
> compiling design
 
 ![](https://github.com/YishenKuma/sd_training/blob/main/day13/44.JPG)

> generating netlist

![](https://github.com/YishenKuma/sd_training/blob/main/day13/45.JPG)

> generated netlist
 
##### Checking design
 
keep in mind we have yet to set any constraints on the design, and any constraint that may be present in loaded from the DC tool memory.
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/36.JPG)
 
>  check_design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/37.JPG)
 
> check_timing
 
####  Compiling vsdbabysoc
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/50.JPG)
 
> error encountered in reading verilog file due to the real elements that are not synthesizable
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/51.JPG)
 
> real need to be changed to reg, or removed
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/52.JPG)
 
> reading in design after appropriate changes made
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/53.JPG)
 
> compiling design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/54.JPG)

> generated netlist
 
##### Checking design
 
keep in mind we have yet to set any constraints on the design, and any constraint that may be present in loaded from the DC tool memory.
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/56.JPG)
 
>  check_design
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/57.JPG)
 
> check_timing
 
#### Post synthesis simulation to check mismatch between RTL and GLS
 
![](https://github.com/YishenKuma/sd_training/blob/main/day13/27.JPG)

> vcs  gls.v sky130_fd_sc_hd.v primitives.v
 
Error encountered pending debug

</details>
	
## **Day_14: Synopsys DC and Timing Analysis**

<details><summary> Lecture Day 14 </summary>

* Corners of PVT

PVT refers to process, voltage, temperature

> Process: refers to the variation I the parameters of transistors during fabrication, as layers getting fabricated cannot be uniform across the die

> Voltage: refers to the varying voltages on chip during operation, can be cause by few reason such as IO drop or supply noise from parasitic inductance

> Temperature: refers to the varying temperature of chip during operation due to power dissipation in the MOS-transistors  which will affect the delay on the cells

![](https://github.com/YishenKuma/sd_training/blob/main/day14/1.JPG)

> effect of PVT on the delays introduced on circuit

IC chips are designed such that that can function in a wide variety of temperatures and voltages. For this reason, the must simulate the design at different conditions of PVT. These conditions are known as corners. 

#### Timing Terminologies

The values below show how the deisgn could be missing the timing requirements. Looking at these values will help us in optimizing design. 

* WNS

 Worst negative slack – refers to the slack of the path with the worst timing failure, if WNS is positive, it means that the path has passed, if it is negative then it has failed. Refers to setup time.

* WHS

Worst hold slack – refers to the slack of the hold path with the worst timing failure. 

* TNS

Total negative slack – sum of the total negative path slacks, or the sum of all WNS

* THS

Total hold slack – sum of the total negative hold slack paths, of the sum of all WHS 

</details>
	
<details><summary> Lab Day 14 </summary>

#### Using Timing Libs for different PVT corners

![](https://github.com/YishenKuma/sd_training/blob/main/day14/101.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day14/102.JPG)

> cloning the libs into directory

![](https://github.com/YishenKuma/sd_training/blob/main/day14/103.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day14/104.JPG)

> schematic design of the babysoc 

![](https://github.com/YishenKuma/sd_training/blob/main/day14/105.JPG)

> inputs and outputs of design

![](https://github.com/YishenKuma/sd_training/blob/main/day14/106.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day14/a.JPG)

> clock is not a port in this design as the clk is genertated by pll, so to create the clock, we will use the pins uut2/CLK, which is the output of PLL

![](https://github.com/YishenKuma/sd_training/blob/main/day14/107.JPG)

> constraints set for design, constrains are set tightly to have the paths violated to see the effect of the different PVT corners.

![](https://github.com/YishenKuma/sd_training/blob/main/day14/108.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day14/109.JPG)

> error in reading lib files for PVT corners, these errors haver to be resolved before the lib file can be read and the conversion to db can be done by lc_shell

![](https://github.com/YishenKuma/sd_training/blob/main/day14/110.JPG)

> cross checking lib file that give error with successfully read lib file and making corrections based on that

![](https://github.com/YishenKuma/sd_training/blob/main/day14/111.JPG)

> lib file successfully converted to db, now we repeat this to get the dbs for alkl PVT corner lib files

#### Documentation of different PVT corners

![](https://github.com/YishenKuma/sd_training/blob/main/day14/108.JPG)

> using the command report_qor to get the value of wns, tns, whs, ths

![](https://github.com/YishenKuma/sd_training/blob/main/day14/113.JPG)
 
Steps to use in dc shell for each timing lib file
 
> set target_library {/nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/rvmyth/vsdpcvrd/resources/timing_libs/<timing_lib.db> /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsddac.db /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsdpll.db}
	#change target and link library
	
> set link_library {* /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/rvmyth/vsdpcvrd/resources/timing_libs/<timing_lib.db> /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsddac.db /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsdpll.db}

> read_file {mythcore_test.v avsd_pll_1v8.v avsddac.v clk_gate.v vsdbabysoc.v} -autoread -format verilog -top vsdbabysoc

> source cons.tcl 

> link

> compile

>report_qor #to get the WNS WHS THS

> now we read in all the converted libs to check the values for the different PVT corners

*lib_file* | *wns* | *whs* | *tns* | *ths*
--- | --- | --- | --- | ---
sky130_fd_sc_hd__tt_025C_1v80 | 0.60 | 0.09 | 547.98 | 8.45
sky130_fd_sc_hd__ff_100C_1v65 | 0.10 | 0.15 | 69.02 | 87.96
sky130_fd_sc_hd__ff_100C_1v95 | 0.00 | 0.20 | 0.00 | 222.95
sky130_fd_sc_hd__ff_n40C_1v56 | 0.48 | 0.11 | 440.36 | 13.98
sky130_fd_sc_hd__ff_n40C_1v65 | 0.21 | 0.14 | 174.23 | 69.26
sky130_fd_sc_hd__ff_n40C_1v76 | 0.02 | 0.18 | 5.25 | 142.57
sky130_fd_sc_hd__ss_100C_1v40 | 4.50 | 0.00 | 5489.95 | 0.00
sky130_fd_sc_hd__ss_100C_1v60 | 2.60 | 0.00 | 3044.51 | 0.00
sky130_fd_sc_hd__ss_n40C_1v28 | 11.75 | 0.00 | 15530.87 | 0.00
sky130_fd_sc_hd__ss_n40C_1v35 | 7.80 | 0.00 | 10208.25 | 0.00
sky130_fd_sc_hd__ss_n40C_1v40 | 6.57 | 0.00 | 8380.09 | 0.00
sky130_fd_sc_hd__ss_n40C_1v44 | 5.87 | 0.00 | 7114.41 | 0.00
sky130_fd_sc_hd__ss_n40C_1v76 | 1.90 | 0.00 | 1982.41 | 0.00

</details>	

## **Day_15: Inception of EDA and PDK**

<details><summary> Lecture Day 15 </summary>

#### Introduction to QFN-48 Package, chip, pads, core, die and IPs

* Package

![](https://github.com/YishenKuma/sd_training/blob/main/day15/1.JPG)

The flat no leads packages, surface mount technologies, are used to physically and electrically connect ICs to PCBs. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/2.JPG)

The chips sit sin the centre of the package, wire bonds are used for the connectivity between the package and the chip, allowing the external signals into the chip. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/3.JPG)

The elements within the package include:

* Pad: intermediate structures connecting the internal signals from the core of IC to the external pin of the chip, prevents external charges from damaging the core inside

* Core: the section of the chip where the fundamental logic of the design is placed (Macros, IPs, Etc,.)

* Die: the die refers to the square of silicon containing the integrated circuit 

* Foundy IPs: Macro cells developed with the intent of licencing to multiple vendor for using as building blocks in different chip designs, known as Intellectual Property

* Macros: Simple custom built cell serving a specific functional purpose that can be found through open sources

#### Introduction to RISC-V

RISC-C is an ISA (instruction set architecture), which is a language which allows us to talk to the computer. If we want a pass a particular information to the hardware of computer, we need top translate this information into a binary format which is readable by the hardware. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/4.JPG)

For example, we want to run a c program. The c commands will first be compiled into assembly language. The assembly language will be converted into the binary format or machine language. This can be read by the hardware to give us the desired output. But we may need to implement the HDL (hardware description language) interface between the RISC-V architecture and the layout, in order to implement the RISC-V specifications through RTL.

#### From Software Applications to Hardware

![](https://github.com/YishenKuma/sd_training/blob/main/day15/5.JPG)

The application software will enter into the system software block before going into the hardware, the system software is where the conversion into binary language takes place. The System software components icnlude the Operating System (OS),  Compile and assembler.

* OS

Handles IO operations, allocates memory, handles low level system functions, and convert the assembly language of application software and convert into binary language. 

* Compiler

![](https://github.com/YishenKuma/sd_training/blob/main/day15/7.JPG)

Converts the programming language (C, C++, Java, …) into their respective instructions. These instructions act as an abstract interface between the programming language and the hardware, which is also known as the Instruction Set Architecture (ISA), or the “architecture of the computer”. The RTL description language which implements the instruction set, can then be synthesized to then produce the synthesized netlist, then the physical design implementation of the netlist. 

* Assembler

Takes in the instructions output by the compiler and produces the binary language for the hardware to read

![](https://github.com/YishenKuma/sd_training/blob/main/day15/6.JPG)

> example of the flow in the case of a stopwatch application

#### all components of open-source digital asic design

![](https://github.com/YishenKuma/sd_training/blob/main/day15/8.JPG)

In order to design ASICs, we require HDL including the RTL IPs, EDA tools, and the Process Design Kit (PDK). 

* PDK

Process Design Kits are the interface between the Fab and the designer, instead of having the design being tightly integrated with the manufacturing.

The PDK Includes process design rules (DRC, LVS, PEX), device models, digital standard cell libraries, IO libraries, etc. 

* EDA Tools 

LVS, DFT, DFM, Power Planning, CTS, STA, Detailed Routing, RTL synthesis, FLoorplanning, etc.

ASIC design requires many steps ad the process is very complex, as such, a methodology is needed. The methodology is implemented through the RTL to GDSII flow

#### Simplified RTL to GDSII Flow

![](https://github.com/YishenKuma/sd_training/blob/main/day15/9.JPG)

The flow begins with the RTL model and ends with the ready to fabricate masked set layout in the GDSII format. 

The major steps in the flow is:

* Synthesis: 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/10.JPG)

The RTL model is converted to a circuit out of components based on the standard cell libraries, resulting circuit is referred to as the gate-level netlist

![](https://github.com/YishenKuma/sd_training/blob/main/day15/11.JPG)

The standard cells within the standard cell libraries have regular layout, and have different models or views. 

* Floorplanning

Objective is to plan the silicon area and create robust power distribution network. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/12.JPG)

In Chip floor-planning,  the chip die is partition between different system building blocks, and the I/O pads are placed

![](https://github.com/YishenKuma/sd_training/blob/main/day15/13.JPG)

In macro floorplaning, the dimensions, pin locations and rows are defined

![](https://github.com/YishenKuma/sd_training/blob/main/day15/14.JPG)

In power planning, the power network is constructed. Typically, the chip is powered by multiple ground and VDD pins, the power plans are connected to components through rings and straps, the parallel connections are meant to avoid high resistance and address electromigration problem.  The network will typically use upper metal layers as compared to lower metal layers as they are thicker. 

* Placement

![](https://github.com/YishenKuma/sd_training/blob/main/day15/15.JPG)

In this step, the cells are placed in the floorplan rows, aligned with the sites. Macros would be placed through placing gate level netlist cells on the rows and very close to each other to reduce interconnect delays and enable successful routing.

![](https://github.com/YishenKuma/sd_training/blob/main/day15/16.JPG)

Placement will be done through 2 methods, Global and Detailed. Global placement tries to find optimum placement for all cells, the positions are not necessarily legal and cells may overlap. In detailed routing, the placements from global placement is modified such that the placement of cell will become legal 

* Clock Tree Synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day15/17.JPG)

Purpose of the step is to deliver all the clocks to all the sequential elements with minimal skew and in good shape. 

* Routing

![](https://github.com/YishenKuma/sd_training/blob/main/day15/18.JPG)

In this step, the interconnect nets are implemented through the available metal layers. The metal tracks from the routing grid. As the routing grid is usually huge, the design is usually divided and concurred. Global routing will generate the routing guides, then detailed routing implements the wiring according to the routing guides. 

* Sign-Off

The final step in the flow, where the final layout is constructed, and we perform Physical and Timing verifications. The layout needs to honour design rules, match with the original gate-level netlist, timing constraints are met, and  design is operating at desired frequency. 

#### Introduction to OpenLANE and Strive chipsets

When doing open source ASIC flow, we need to be wary of the tool qualification, tool calibration and any missing tools. With the release of open source PDK, a reference open source ASIC implementation with dogm flow was created, and is known as open lane. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/19.JPG)

Openlane is free to use, open-source, comes with the apache 2.0 liscence, and has a public github repo. Started as an an Open-Surce Flow for a True Open Source Tape-Out Experiment. There is an open PDK, open RTL and open EDA.

He main goal for open lane is to create clean GDSII, no lvs drc and riming violations, without human intervention.

OpenLANE can be used to harden macros and chips. 

OpenLANE flow can be operated either autonomous or interactively. 

One of openlane features include design space exploration, where the best set of flow configurations can be found. 

#### OpenLANE detailed ASIC design flow

![](https://github.com/YishenKuma/sd_training/blob/main/day15/20.JPG)

The ASIC lane flow has several steps, starts with the design RTL and ends with the GDSII layout. Flow starts with RTL synthesis, using yosys with constraints which translates the design intop logic circuit. The circuit can be optimized and then mapped using abc, which must be guided by the optimization, which comes in the form of abc scripts, Open lane comes with several abc scripts, referred to as syntesis strategies. Different designs can use different strategies to achieve objectives, for that we have the synthesis exploration.

* Synthesis Exploration and Design Exploration

![](https://github.com/YishenKuma/sd_training/blob/main/day15/21.JPG)

The synthesis exploration is used to generate reports that shows how the design delay and area is affected by the strategy. We can pick the best strategy based on this exploration. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/22.JPG)

Openlane also has design exploration utility which can be used to sweep the design configurations and generates a report similar to the one shown above, showing different design matrix, which is also useful to find the best configuration for a design. Deisgn exploration can alkso be used for regression testing (CI).

* DFT

![](https://github.com/YishenKuma/sd_training/blob/main/day15/23.JPG)

After synthesis, we need to perform DFT so our design will be ready for testing after fabrication. This step uses the open source project known as fault. Within the DFT step, the design undergoes scan insertion, Automatic Test Pattern Generation (ATPG), Test Patterns Compaction, Fault Coverage, Fault Simulation. Essentially, additional logics will be added which allows testing after fabrication. 

* Physical Implementation

This stage is also known as place and route, wherein the tool performs, floor/power planning. End coupling capacitors and tap cells insertion, global and detailed placement, post placement optimization, clock tree synthesis, and global routing and detailed routing. 

* Die Insertion

During physical implementation, we have die insertion, this step is required to handle the antenna rule violations.

![](https://github.com/YishenKuma/sd_training/blob/main/day15/24.JPG)

Antenna rule violation refers to a rule that is necessary in order to avoid antenna effect. Antenna effect refers to when metal wire segments are fabricated, they can act as an antenna if the wire segment length is too long. Reactive ion etching can cause charges to accumulate on the wire, and this charge will may cause the transistor gates to be damaged during fabrication. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/25.JPG)

One way to handle this is by performing bridging which attaches a higher layer to act as an intermediary, which requires router awareness. Second method is by adding an antenna diode cell to leak a way the accumulated charges.

![](https://github.com/YishenKuma/sd_training/blob/main/day15/26.JPG)

For open lane, a different method is used, where a fake antenna diode is added next to ecery cell input after placement. The antenna checker is run on the routed layout. If the checker reports a violation on the cell input pin, the Fake diode cell will be replaced by a a real one. 

* LEC (Logic Equivalence Check)

Since we perform optimization, which involves some transformation during physical implementation, we need to check the logic equivalence between the netlist using yosys, to make sur e the design is functionally equivalent. Whenever the netlist is modified, such as during CTS or Post placement, verification needs to be performed. 

* Signoff

This step involves Static Timing Analysis (STA), Design Rule Checking (DRC), and Layout versus Schematic (LVS). 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/27.JPG)

STA involves timing reports to check violations in timing paths. 

Physical verification involves DRC and LVS, Magic is used for DRC and SPICE Extraction from layout, Magic and Netgen are used for LVS, where extracted PSICE by Magic vs verilog netlist are used. 

</details>
	
<details><summary> Lab Day 15 </summary>

#### OpenLANE Directory structure in detail

![](https://github.com/YishenKuma/sd_training/blob/main/day15/51.JPG)

> Within the openlan working directory, we have the openlane directory which we will work in ,aand the pdk directory which contains all the skywater pdk, open pdks and sky130A. The skywater pdk has all the psk related files, which has the timing libraries, the lef files, the tech lefs, etc. The reason of having the open pdks consists of scripts and files that converts the foundry level pdks to be compatible with the open source eda, such as Magic or Netgen. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/52.JPG)

> Sky130A is the pdk which has been made compatible with the open source environment. Within this directory we have libs.ref and libs.tech.  Libs.ref contains all the process specific files, while libs.tech contains tool specific files. 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/53.JPG)

> here we can see all the timing libs we will be using. 

#### Design Preparation Step

![](https://github.com/YishenKuma/sd_training/blob/main/day15/54.JPG)

> to run the complete flow, we run the flow.tcl command without any switches

![](https://github.com/YishenKuma/sd_training/blob/main/day15/55.JPG)

> We need to require the packages every time we run

![](https://github.com/YishenKuma/sd_training/blob/main/day15/56.JPG)

> These are the designs that we have

![](https://github.com/YishenKuma/sd_training/blob/main/day15/57.JPG)

> src hold the verilog files which will be used as well as sdc information

![](https://github.com/YishenKuma/sd_training/blob/main/day15/58.JPG)

> config.tcl bypasses any configurations that were done in default flow

![](https://github.com/YishenKuma/sd_training/blob/main/day15/59.JPG)

> error encountered during prep command

![](https://github.com/YishenKuma/sd_training/blob/main/day15/60.JPG)

> we must use the command make mmount to invoke openlane 

![](https://github.com/YishenKuma/sd_training/blob/main/day15/61.JPG)

> design setup stage performed 

#### Review files after design prep and run synthesis

![](https://github.com/YishenKuma/sd_training/blob/main/day15/62.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day15/63.JPG)

> now we have the runs directory created

![](https://github.com/YishenKuma/sd_training/blob/main/day15/64.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day15/65.JPG)

> information within the .lef generated

![](https://github.com/YishenKuma/sd_training/blob/main/day15/66.JPG)

> config.tcl shows all the default directories taken by the run

![](https://github.com/YishenKuma/sd_training/blob/main/day15/67.JPG)

> cmds.log shows all the command used

![](https://github.com/YishenKuma/sd_training/blob/main/day15/68.JPG)

> running synthesis using run_synthesis command 

#### OpenLANE Project Git Link Description

https://github.com/efabless/OpenLane

> we can see all the info on OpenLane in the github linked above

#### Steps to characterize synthesis results

> STA, synthesis and abc has been performed

![](https://github.com/YishenKuma/sd_training/blob/main/day15/69.JPG)

> chip are for module

![](https://github.com/YishenKuma/sd_training/blob/main/day15/70.JPG)

> The flop ratio is the number of D flip flops against total number of cells, flop ratio would be 1613/14876 x 100= 10.84

 ![](https://github.com/YishenKuma/sd_training/blob/main/day15/71.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day15/72.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day15/73.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day15/74.JPG)

> reports generated

</details>
	
## **Day_16: Understand importance of good floorplan vs bad floor plan and introduction to library cells**

<details><summary> Lecture Day 16 </summary>

#### Utilization factor and aspect ratio

* Define width and height of core and die

![](https://github.com/YishenKuma/sd_training/blob/main/day16/1.JPG)

We begin with the netlist that defines the connectivity between all the cells, the dimensions of the chip is dependant on the dimensions of the logic gates, 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/2.JPG)

The logic gates will be represented as cells with respective dimensions

![](https://github.com/YishenKuma/sd_training/blob/main/day16/3.JPG)

With these dimensions we can calculate the area occupied by the netlist on the IC chip

![](https://github.com/YishenKuma/sd_training/blob/main/day16/4.JPG)

If the logic completely utilizes the area available on the chip, then we have 100% utilization, or a utilization of 1.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/5.JPG)

The aspect ratio signifies the shape of the chip, if the ratio is 1, then the chip shape is square.

#### Concept of pre-placed cells

![](https://github.com/YishenKuma/sd_training/blob/main/day16/6.JPG)

Preplace cells refer to cells which are implemented once and can be instantiated multiple times onto one netlist, as this is part of the top-level netlist, such us IP’s memory, comparator, etc. The placement of these cells have to be done before placement and routing. The arrangement of these cells on chip is referred as floorplannning, based on user defined locations. 

Automated placement and routing tools will place the remaining logical cells in the design onto chip. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/7.JPG)

Preplace cells can also refer to blackboxes, where the netlist has been separated out and becomes invisible to the top netlist, so the user can instantiate the block multiple times while only implemented once.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/8.JPG)

The locations of the preplace cells must be well defined.

#### De-coupling capacitors

![](https://github.com/YishenKuma/sd_training/blob/main/day16/9.JPG)

In any circuit, whenever there is switching activity occurring, the circuit demands switching current. Whenever there is switching, there will be a capacitive discharge occurring, and the discharge current should be handled well by the power supply coupling.  However, due to the presence of Rdd and Ldd, there will be a voltage drop, so the value of voltage will be slightly lower than the main supply. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/10.JPG)

The value of the reduced voltage must be within the noise margin range so that the transition of logic to be detected. For signal to be considered as logic 1 ort 0, it should be in the NMl and NMh ranges respectively. If the value of our voltage drop is too great, our signal could fall into the undefined region which would not be good, so this is where we use the decoupling capacitors. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/11.JPG)

The decoupling capacitor connected in parallel with the circuit, provides current to the circuit during switching activity. The RLL network will be used to replenish the charge into the decoupling capacitor when there is no switching activity. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/12.JPG)

Placement of decoupling capacitors.

#### Power Planning

![](https://github.com/YishenKuma/sd_training/blob/main/day16/13.JPG)

For sending signals between blackboxes, we cannot always be having decoupling capacitors to be inserted to handle the potential voltage drop for the switching activity.  As the power supply is coming from one source, there is a change of the signal having aground bounce or a voltage sloop.  

![](https://github.com/YishenKuma/sd_training/blob/main/day16/14.JPG)

How we handle this is by having multiple power source lines, this way, whenever there is switching activity, the power will be taken from the nearest power line. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/15.JPG)

This is what is known as power grid mesh that is used in the power planning stage.

#### Pin placement and logical cell placement blockage

![](https://github.com/YishenKuma/sd_training/blob/main/day16/16.JPG)

The connectivity information between the gates is coded using the VHDL/Verilog language and sis called as the netlist. The above circuit shown has 4 input pins and 4 output pins, 2 input clk ports and 1 output clk port. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/17.JPG)

Pin placement is dependent on the functionality of the design, backend team will be responsible for this. Clock ports are also larger due to design being driven by these clcock paths, so we need these paths to have as low resistance as possible. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/18.JPG)

There needs to be a logical cell placement blockage, so that no cells are inserted and there will be no overlaps between the pins. 

#### Netlist binding and initial place design

![](https://github.com/YishenKuma/sd_training/blob/main/day16/19.JPG)

We need to bind the netlist of the physical cells, the cells will have a real view of a box with a specific width and height. These boxes will be available in a library file, having the widths and heights of the cells, as well as other details such as delay or required information, as well as the flavor of the cells. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/20.JPG)

During placement stage we must ensure that the area used for the blackboxes and deccaps cells do not have any cells inserted and cause overlaps. The placement needs to be timing conscious as well to not make the routing long.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/21.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day16/22.JPG)


![](https://github.com/YishenKuma/sd_training/blob/main/day16/23.JPG)

We will then need to optimize this placement. We do this through wire length and capacitance estimation. One way is through signal integrity through signal repeaters, which are buffers that recondition old signal and reproduces the signal to the following stage to maintain signal integrity, however this comes at the cost increase area. 

#### Need for libraries and characterization

Logic synthesis is needed to convert the functionality in terms of RTL into functionality in terms of hardware. The output will be an arrangement of gates that will represent the original functionality. Then we perform floorplanning where the shape of the design is made based on user specification asnd the placement of pre-placed cells. Then we perform placement such that the placement of the cells is meeting the intended timing of the design. Next we perform CTS, to have no timing issues for the in terms of the clock endpoints. Lastly, we perform routing, where the routing needs to take into factor the properties of the cells. Then we have STA, in which we do timing analysis, and checks for hold and setup timings. 

The common thing in all these stages are the gates. This is where the library calculation is step is very important. The gates must be modelled such that the tool can understand what the gate is and the timing characteristic of the gates. 

#### Inputs for cell design flow

![](https://github.com/YishenKuma/sd_training/blob/main/day16/24.JPG)

The library holds all the standard cells and information with different functionality, threshold voltages, sizes. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/25.JPG)

> design rules

The inputs for the cell design flow are the PDKS, DRC and LVS rules, spice models, library and user defined specs. The rules have been tested and set based on the foundrys. There will be more than thousands of design rules that the cell must follow. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/26.JPG)

> spice models given by foundry

![](https://github.com/YishenKuma/sd_training/blob/main/day16/27.JPG)

> library and user defined specs incled cell height, supply voltage, metal layers, drawn gate length and pin location.

The design stage involves 3 stages, circuit design, layout design and characterization. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/28.JPG)

Circuit design involves implementing the function, and then model the transistors to meet the library requirements which are based on spice simulations. Then once we have the values of W/L of the mos, we implement the values in the layout. The typical output we get from circuit design is the CDL, which is the circuit description language. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/29.JPG)

The first step in layout design is to get the function implemented through a pmos and nmos transistors, then get the pmos and nmos network graphs. 

#### Layout Design Step

The art of layout is the euler’s path and the stick diagram

![](https://github.com/YishenKuma/sd_training/blob/main/day16/30.JPG)

After you get the pmos and nmos network path, you open the euler’s path. The euler’s path is basically a path that has only been traced once.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/31.JPG)

The next step would be to draw a stick diagram of it. A C E F D B are nothing but the inputs, the connections are made being mentioned by the circuit. This will detail the connec6ions for the source and drains for the mos transistors of the input pins. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/32.JPG)

Then we convert this stick diagram into a layout based on the drc rules given by the foundry, and the top level specifications by the user.  

Lastly we extract the parasitics of this layout and characterize it in terms of timing. The characterization is helpful to get the timing, noise and power information. 

The final outputs of the cell design flow will be the CDL (circuit description langauge), gdsii, lef, extracted spice netlist (.cir) , Timing, noise, power .libs, function

#### Typical characterization flow

Now we have our outputs in the terms of a extracted spice netlist and spice models. 

Firstly we read in the spice models and the tech file from the layout.

The second step is to read in the extracted spice netlist. 

The third step is to recognize the behaviour of the buffer.

The fourth step is to read in the subcircuit of the inverter.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/33.JPG)

Then you need to attach the necessary power sources.

The sixth step is to apply the stimulus, and the output capacitance is the seventh step.

The eight step is to provide the simulation command. 

The next step is to feed in all the inputs for the previous 8 steps in the form of a config file through the characterization software GUNA. This software will generate the timing, noise, power .libs, function. 

The classification of .libs is based on the timing, noise and power characterization. 

#### Timing threshold definitions

![](https://github.com/YishenKuma/sd_training/blob/main/day16/34.JPG)

These are the variables related top any waveform seen. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/35.JPG)

Slew low rise thr refers to the defined value of the graph closer to zero, typically at 20%. But this is not enough to calculate the slew, you need the slew high rise thr as well. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/36.JPG)

For the high rise thr you take the value of 20% from the top. So to get the slew, you will us ethese to points over the timing difference. 

Similar definition applies for the falling waveform.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/37.JPG)

We also have thresholds for the delays. In rise thr refers to the best defined point to calculate the delay. Similarly we have the out rise thr at the 50% mark, if we want to calculate the delay of the cell, we need to take the time period between the 2 points. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/38.JPG)

Similarly, for a fall waveform, the definition applies the same but for the fall waveform.

#### Propagation delay and transition delay

![](https://github.com/YishenKuma/sd_training/blob/main/day16/39.JPG)

If we want to calculate the delay, we only need to subtract out minus in, the time at the out thr minus the time at the in thr. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/40.JPG)

For an example shown above, it is very easy to get the delay by subtracting the time. There will exist a problem if there is a moment of the threshold.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/41.JPG)

If by chance the threshold moves, and the output moves and becomes before the input, then our delay will become a negative value, qhixh should not be seen, and would be a result of poor choice of threshold point. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/42.JPG)

Another reason we might get a negative delay is if we get a waveform as above. Form the slew of the input waveform, we can undertsand that the delays on the input wires are quite high. Even with the proper choice of thr point, its will still give a value of negative delay, so the deisgn of the circuit is also very important. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/43.JPG)

For transition time, we need to subtract the time of slew high rise thr minus the time of slew low rise thr for rise waveform. The similar case applies for the fall waveform, using the slew low and high for fall. 

</details>
	
<details><summary> Lab Day 16 </summary>

#### Steps to run floorplan using OpenLANE

![](https://github.com/YishenKuma/sd_training/blob/main/day16/101.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day16/102.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day16/103.JPG)

Within the configuration directory, there will be a README.md file which has the switches of the tool to use during stages. These switches are set in the .tcl files in the configuration directory. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/104.JPG)

These are the system default settings, which is the lowest priority for the tool, the highest priority is in the design directory, the config.tcl and the pdk variant config.tcl. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/105.JPG)

We run the floorplan stage using “run_floorplan”

#### Review floorplan files and steps to view floorplan

![](https://github.com/YishenKuma/sd_training/blob/main/day16/106.JPG)

We can see our variable for the core utilization is set to 35.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/107.JPG)

The highest priority file that sets this value over the other file is the pdk variant config.tcl	

![](https://github.com/YishenKuma/sd_training/blob/main/day16/108.JPG)

To view the floorplan, we must use the .def file within results directory. We can see the coordinates of the core area specified. If we divide the numbers by 1000, we will have the area of the chip in micrometers. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/109.JPG)

We use the command “magic -T /Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130.tech lef read /Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/17-01_06-56/tmp/merged.lef def read /Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/17-01_06-56/results/floorplan/picorv32a.floorplan.def &”

#### Review floorplan layout in Magic
![](https://github.com/YishenKuma/sd_training/blob/main/day16/109a.JPG)

Hit s on the keyboard to select and hit v to maximize the design. Left click and right click to select a region. z and shift z to zoom in and zoom out.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/110.JPG)

Here we can see the input pins 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/111.JPG)

Hitting s key and checking the tkcon window, use the command “what” to see the cell information.

The decap cells have been arranged along the side rows of the design as end cap cells. And there are are also tap cells meant to avoid the latch up conditions that occur in the cmos devices. The taps cells are placed of equal distance.

![](https://github.com/YishenKuma/sd_training/blob/main/day16/112.JPG)

The standard cells are placed at the bottom left corner of the design, it will only be placed during placement stage. 

#### Congestion aware placement using RePlAce

![](https://github.com/YishenKuma/sd_training/blob/main/day16/114.JPG)

We perform the placement using command “run_placement”. 

![](https://github.com/YishenKuma/sd_training/blob/main/day16/115.JPG)

We look at the design after placement with the command “magic -T /Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130.tech lef read /Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/17-01_06-56/tmp/merged.lef def read /Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/17-01_06-56/results/placement/picorv32a.floorplan.def &”

![](https://github.com/YishenKuma/sd_training/blob/main/day16/113.JPG)

All the std cells have been placed.

</details>
	
## **Day_17: Design and characterise one library cell using Layout tool and spice simulator**

<details><summary>  Lecture Day 7  </summary>

<details><summary> SPICE deck creation for CMOS inverter </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/1.JPG)

The first step in performing the spice simulations is to create the spice deck. The spice deck holds the connectivity information of the netlist and other information. We need to have specified for the spice deck the component connectivity, component values, node of the design, node names. .dc is used to perform the simulation, the command shown above is used to sweep the input voltage from 0 to 2.5 at steps of 0.05, and measure output voltage while we sweep the input voltage.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/2.JPG)

 The final step is to describe ethe model file with the command .lib, with this command we create the model file which has all the information described in the top part.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/3.JPG)

The spice model will look as shown above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/4.JPG)

The simulated file waveform achieved in ngsipice using the commands [source “modelfile”.cir > run > setplot > dc1 > plot out vs in ]. This waveform is based on the modelling of the wn=wp=0.375u, ln=lp=0.25. The waveform shows the characteristics of the transistors. The waveform however can be noticed shifted slightly to the left. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/5.JPG)

Now we run the waveform, but this time we do the modelling of wn= 0.375u, wp=0.9375u, ln=lp=0.25. The wp/lp =2.5 while the wn/ln = 1.5. Now we can see the graph is not shifted to the left and is in centred. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/6.JPG)

The reason why the graph is not shifted for the voltage shifting of the design which the pmos width is larger than the design where the widths of nmos and pmos are the same, is because the cmos circuit constructed is more robust. One of the parameters that defines the cmos inverter robustness is the switching threshold, Vm, which is the voltage when Vin = Vout. For the case of wn/ln=wp/lp=1.5, our Vm is 0.9v. For the case of wn/ln=wp/lp=3.75, our Vm is 1.2v.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/7.JPG)

The point where the vin=vout is when both transistors are in saturation region, where there is a high chance of leakage.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/8.JPG)

When the vin=vout, the gate voltage is equal the the drain voltage, so the vgs will be very little compared to threshold voltage. At the point where vgs=vds, the currents idsn and idsp will be the same, just flowing in opposite directions. 

</details>

<details><summary> Static and dynamic simulation of CMOS inverter </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/9.JPG)

In order to do dynamic simulation, where we can analyse the rise and fall delay and how it varies with the switching threshold, we use a pulse wave as an input, and the simulation command will be a transient analysis. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/10.JPG)

The pulse graph will start from 0, rises until 2.5 v, falls until 0, pulse width is 1 ns and complete cycle is 2ns

![](https://github.com/YishenKuma/sd_training/blob/main/day17/11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/12.JPG)

The rise delay calculation is based on the 50% point,  the difference in time between when the falling input crosses 50% and the point where rising output crosses 50%. The fall delay calculation is based on the 50% point,  the difference in time between when the rising input crosses 50% and the point where falling output crosses 50%.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/13.JPG)

For the design with wp/lp=wn/ln, we have the rise delay and fall delay measured a shown above. 

</details>

<details><summary> CMOS Fabrication process </summary>

<details><summary> Creating active regions </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/14.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/15.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/16.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/17.JPG)

The first step is the 16-mask CMOS fabrication process is selecting a substrate on which the complete design is fabricated onto. The most common type of substrate used is a p-type substrate with high resistivity and orientation <100>.  We also need to ensure substrate has a doping level that is lower than ‘well’ doping. Then we create small pockets in the substrate for the active regions for the transistors. We also need to create isolation between the pockets through the deposit of SiO2 layer on the substrate, and then a layer of Si3N4 on that. Then through the process of lithography, the regions for the pockets is created on the layer through photoresist mask, and etched away to leave the pockets. Then the photoresist is washed off to leave only the etched Si3N4 and the SiO2 layer remain.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/18.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/19.JPG)

Then we can grow the oxides of the exposed areas of the SiO2, while the are under the Si3N4 is protected from growing during the oxidation furnace. This process is known as LOCOS, and the areas created is known as bird beaks. Then the Si3N4 is striped away and that is how we get the isolation regions and active regions.  

</details>

<details><summary> Formation of N-Well and P-Well </summary>

We need to form the n-well and p-well one at a time.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/21.JPG)

We first deposit a layer of photoresist with a masking layer to expose the region which the p-well is formed first. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/22.JPG)

Then we perform the doping process with boron on the exposed area to form the n-well, the reason for why boron is used is due to its bonding property with silicon top create holes. This process is known as ion implantation, the boron is diffused into the substrate, creating an active p area. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/24.JPG)

We do the same for the next same now to create the active n well region using ion implantation with phosphorus. Phosphorus is used due to its bonding properties with silicon to create electrons. Now we have both the n and p wells formed. However the depth of the wells are not finalized yet. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/25.JPG)

Next we take the structure into a driving furnace for a long time so that the boron and phosphorus diffusion will be driven in further into the p-substrate so the wells are formed clearly. In the n-well we will create a p-mos transitor, and in the p-well we create the n-mos transisitor.

</details>

<details><summary> Formation of gate terminal </summary>

Gate by far is the most important terminal for the mos devices because that is what defines the threshold voltage, which is what defines the turn on voltage of the gates. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/26.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/27.JPG)

The Threshold voltage is very dependent on the doping concentration and the oxide capacitance, during the doping steps, we try to control these 2 factors so that we can control the threshold voltage.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/28.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/29.JPG)

Through another masking step, we expose the previous p-well area to undergo diffusion again. We perform ion implantation of boron but this time with lower energy, so the diffusion will be just at the surface. We will use the doping concentration into getting the threshold voltage. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/30.JPG)

We do the same thing on the other side for the n-well. Arsenic has the same elemental properties as phosphorus so it can be used. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/31.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/32.JPG)

During the past few implantation stages, the oxide layer will become quite damaged, to handle this, we etch away the oxide and regrow the oxide layer. The thickness of the oxide can be grown based on the threshold voltage desired, since it is based on the oxide capacitance as well as the dopant concentration. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/33.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/33a.JPG)

A thick polysilicon layer is deposited and dope it with some impurities, as the gate area is supposed to be of low resistance. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/34.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/35.JPG)

Then we add the photoresist layer removed through a mask to create the gate patterns. The gate mask pattern is shown above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/35a.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/36.JPG)

Then the exposed areas of polysilicon can be etched away. And once the resist is removed as well, what is left is seen above. Now we have the low resistance polysilicon gate formed above the p and n well. 

</details>

<details><summary> Lightly doped drain (LDD) formation </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/37.JPG)

Now we want to achieve the doping profiles a s shown above, for the N-well, we want to get a doping profile of P+,P-,N, we have the N-well have the pmos will be so we have the p type source and drain, which is the P+ doping profile, then want to have the lightly doped drain (LDD) for the P-, and we already have the N doping profile in the N diffused area above the N well. Similarlt the P-well, we want the N+, N-,P doping profile. 

The reason why we want the P- and N- doping profiles between the doping profiles is because of 2 reasons, which are the hot electron effect and the short channel effect. 

> Electric field, E = V/d 

For the hot electron effect, when the device size has actually reduced, the general practice is to not redesign the design, so in the case if the electric field, the d decreases and the electric field increases, which can cause the high energy carriers to break the si-si bonds. The risen energy also may be too high that the 3.2eV barrier for Si conduction band and SiO2 conduction band may be crossed and into the oxide layer, which may cause liability. 

For the short channel effect, when moving to a shorter device channel, the drain channel will begin to penetrate the channel area, making it difficult for the gate to control the source and drain current.  

![](https://github.com/YishenKuma/sd_training/blob/main/day17/38.JPG)

First we create another photoresist layer and mask, exposing the Pwell and gate on the right, and since we are creating the N-mos, we need to perform the implantation using an N-type impurity, the concentration of implantation is chosen carefully such that the N- implant doesn’t penetrate into the well, N- denotes a light dosage of implantation, and the gate protects the channel area from being exposed to the implantation. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/39.JPG)

Next we do the same for the N well, in creating the lightly doped P- regions. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/40.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/41.JPG)

We also have to protect the newly created doped drains, as when we try to generate the actual source and drain, the doped drains structure might get disrupted. So to do this we create some side wall spaces through anisotropic etching, which is a directional etching, so everything will be etched off except for the side walls, creating the side wall spacers. The further implantation will only be impacted on the exposed regions beside the side wall spacers. 

</details>

<details><summary>  source and drain formation  </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/42.JPG)

The next step is to add a thin layer of silicon oxide, this is to avoid the effect of channelling, where we protect the substrate from getting any diffusion during the ion implantation stage. With the layer of silicon oxide, we try to randomize the direction of the ions during ion implantation. 
 
![](https://github.com/YishenKuma/sd_training/blob/main/day17/43.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/44.JPG)

Then we expose the are for the N-mos to perform ion implantation of arsenic to create the N+ source and drain while keeping the LDD intact through the side wall spacers created in the previous step.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/45.JPG)

Then we do the same for the p-mos as well.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/46.JPG)

Then we heat the structure in the driver furnace, exposing to high temperature annealing, to cause the diffusion to go even deeper into the substrate, forming the source and drains.

<details><summary> Local interconnect formation  </summary>

The contacts are very important for user to control the characteristic of the mos devices.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/47.JPG)

First the thin screen oxide is removed using HF solution to open up the areas for contact building.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/48.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/49.JPG)

We need to deposit titanium on the wafer surface through sputtering. Sputtering is the process of hitting the titanium layer with argon gas, so the titanium particles will get removed out and sputtered onto the substrate. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/50.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/50a.JPG)

Then we heat this structure to cause a reaction and create the contact between the titanium and the substrate, which will result in the low resistant TiSi2 being formed. As you can see the regions of titanium in contact with the silicon will react with the silicon. There is also the reaction between the titanium and the nitrogen ambient resulting in TiN which is only used in local communication. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/51.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/52.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/53.JPG)

Through the lithography process and the etching process using RCA cleaning, we leave the TiSi internal connects and the TiN local interconnects.  

</details>

<details><summary> Higher metal level formation </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/54.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/55.JPG)

The steps in the higher metal level formation are the same as the previous step. In regards with the current metal topography, it cannot be used for the reason being there are some problems in terms of the metal discontinuity, so we need to planarize it. This is done firstly by depositing a thick layer of SiO2 that has been doped with phosphorus or boron, phosphorus to protect the sodium ions, and boron to reduce the temperature. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/56.JPG)

Then we undergo chemical mechanical polishing to planarize the wafer. Now we are ready to go for the higher metal level interconnects. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/57.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/58.JPG)

We do so by drilling some contact holes through lithography and etching, making the TiN and the TiSi2 accessible to the top layers. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/59.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/60.JPG)

Then a thin layer of TiN is deposited and a blanket tungsten (W) layer is deposited, which helps us by creating the contact from the bottom to the top. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/61.JPG)

Then through CMP we remove the addition tungsten and planarize the surface.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/62.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/63.JPG)

Then through masks we bring these contact rules outside the chip. We use Al as the metal layer to connect the tungsten holes. Then we mask it to later take it to the higher metal layers. We have aluminium regions in contact with the tungsten holes, which is the second layer of metal. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/64.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/65.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/66.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/67.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/68.JPG)

Through the similar steps, we bring the metal to the higher layers through the TiN layer and tungsten contacts created in the holes etched, and then he third level of interconnects is created. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/69.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/70.JPG)

 Then on the last level of the chip we have the top dielectric layer applied to protect the chip. And a final mask will be used will be used to create the etched holes for the contact holes on the layer, connecting the outside of the chip. 

</details>

</details>
	
</details>
	
</details>

<details><summary>  Lab Day 17 </summary>

<details><summary> IO Placer Revision </summary>

We will be using new .lib files to perform the post layout simulation, post characterizing our sample cell, and plugging this cell into the openlane flow for the picorv32a core. 

For the design at the floorplan stage, we can still implement changes on the fly. 

If we want to change the placement of the IO pins to be around the core, instead of being equidistance and placed randomly. There are 4 strategies that are supported by the IO placer, one of the open source eda tools used in the open lane flow. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/101.JPG)

Variable for the IO placer config within the floorplan.tcl file. The value is set to one for random equidistance. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/102.JPG)

To set the floorplan io mode, we need to use the command set ::env(FP_IO_MODE) 2. And run floorplan again. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/103.JPG)

Now from the design, we can see, the placement method has been changed to being non equidistant, the pins have been stacked on top of one another. 

This is the way the changes are made, by resetting the variables and running the flow again. 

</details>

<details><summary> Lab steps to git clone vsdstdcelldesign </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/104.JPG)

Now we will be cloning files so that we can have the lib files that will allow us to create a new cell and plug in that into openlane flow, instead of removing the standard definition and editing with custom definitions. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/105.JPG)

We will first open up the mag file and see the different layers that is used in the building of the inverter. We will be doing the spice extraction as well as the post synthesis spice simulation. We need to have the magic tech file before we can open the mac file. We use the command magic command to view the layout. 

</details>

<details><summary> Lab introduction to Sky130 basic layers layout and LEF using inverter </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/106.JPG)

On the right side we can see the colours which represent the layers which we can choose. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/107.JPG)

We can see the name of the layer in the top right corner by hovering over a layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/108.JPG)

Hovering over an area, selecting and using the command what will tell the user the selected mask layer. This also tells us that the gats of the mos devices are connected. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/109.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/110.JPG)

Clicking s multiple times includes connected devices into the selection as well. 

https://github.com/nickson-jose/vsdstdcelldesign 

The above site will have a detailed explanation on the technology LEF of the inverter, and how to create a std cell through magic, and building a CMOS step by step.

</details>

<details><summary>  Lab steps to create std cell layout and extract spice netlist </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/111.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/112.JPG)

 We can see the drc violations in the top of the magic window. To find out the error, click the drc tab  and hit drc find next error. We need to ensure final design is drc clean. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/113.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/114.JPG)

To perform the spice extraction, we need to create an extraction file, using command “extract all”. Then to create the spice file, we use the command “ext2spice cthresh o rthresh 0” and “ext2spice”

</details>

<details><summary> Lab steps to create final SPICE deck using Sky130 tech </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/115.JPG)

The generated spice file ahowing the pmos and nmos, with the characterization details and connections. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/116.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/117.JPG)

We need to edit the scale in the spile code to reflect the value in the magic tool. We must also include the pmos and nmos lib files. And we need to comment out the subckt and .end line because we want to include the transient analysis controls as well. Supply voltages needs to be defined. The input pulse must also be specified, and the specification for the transient analysis.  The pmos and nmos models must be renamed accordingly as well in order for the paremetres to be correctly taken from the model lib file.  With this the spice deck is final, and we use the command ngspice to run the spice simulation.

</details>

<details><summary> Lab steps to characterize inverter using sky130 model files </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/118.JPG)

Using the command “plot y vs time a” to show the output y while sweeping input a. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/119.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/120.JPG)

To get the rise transition, we take the time between the values at 20% and 80% of the input signal. The input transition time is 0.0424ns.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/121.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/122.JPG)

Similarly, we can get the fall transition through the same method. Our fall transition is 0.0626ns.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/123.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/124.JPG)

The cell rise and fall delay is calculated based on the 50% point. The cell rise delay is 0.355ns.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/125.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/126.JPG)

The cell fall delay is -0.00389ns.

</details>


<details><summary> Lab introduction to Magic tool options and DRC rules </summary>

There are details for using magic in the website https://opencircuitdesign.com/magic/

Magic technology file tells everything that is needed to know about a process, such as connectivity, drc rules, device extraction rule, generating netlist, rules for reading lef and def. 

CIF refers to one of the common output data formats. Stands for caltec intermediate format and is a human readable format. CIF is sometimes used interchangeably with GDS.

The syntax for DRC rules are available in the DRC section. The basic DRC rules are known as edge-based rules. They work by finding the edge or boundary between 2 layers and checking the area in front of or behind of anything that is violating the design rule. 

</details>

<details><summary> Lab introduction to Sky130 pdk's and steps to download labs </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/127.JPG)

In order to import the magic layouts for the exercise, we use the command wget from the specified link. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/128.JPG)

We run magic using the “magic -d XR” command

</details>

<details><summary> Lab introduction to Magic and steps to load Sky130 tech-rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/129.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/130.JPG)

Open the metal3 file through the file tab. We can see a few independent layout geometries.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/132.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/133.JPG)

One of the rules that must be adhered by magic for metal 3 is that via2 must be enclosed by metal 3 by at least 0.065 microns. To see this visually happening in magic, draw a square and selecting the M3contact on the layer panel by hovering an pressing the p key, then with the cursor box around the area, type the command “cif see VIA2”, we will see the via cuts within the M3 contact, they are created based on the rules in the tech file. The distance between the via cut and the edge is will never be smaller than 0.065 as specified by the rules, thus there will be no drc violation. 

</details>

<details><summary> Lab exercise to fix poly.9 error in Sky130 tech-file </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day17/134.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/135.JPG)

Now we load in poly.mag, which is having 34 drc rules violated. One of the rule violations we should be seeing is the poly.9 rule violation “poly resistor spacing to poly or spacing (no spacing) to diff/tap” must be more than 0.480 microns. We need to correct te tech file, so that this rule gets flagged as a drc violation in the magic tool.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/136.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/137.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/138.JPG)

We need to edit the tech file appropriately based on the poly.9 key. No rule was made for distance rule between poly resistor to poly. 

We use the command “tech load sky130A.tech” to automatically read in the newly modified tech rules. Then run command “drc check”, now the spacing rule has been applied and the violation is showing. 

</details>

<details><summary> Lab exercise to implement poly resistor spacing to diff and tap </summary>
	
![](https://github.com/YishenKuma/sd_training/blob/main/day17/140.JPG)

We need to make several copies of the three resistors, because there are a number of varieties of diffusion in tap, and check against p-diffusion, n-diffusion p-tap and n-tap, using the psd and nsd layers.  Now we can see the errors related just for the poly resistance. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/141.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/142.JPG)

The xhr and uhr ploy resistor are showing the violations, but the n-poly resistors are only flagging the distance to n-tap. Ther is only one rule implemented in the rule file for polyres to n-tap. We fix this in the rule file by, changing the violation rule from *nsd to alldiff.

</details>

<details><summary> Lab challenge exercise to describe DRC error as geometrical construct </summary>
	
![](https://github.com/YishenKuma/sd_training/blob/main/day17/143.JPG)

There is a rule type known as cifmaxwidth that checks layers exactly as they appear in gds output even though the layers aren’t something you can draw directly in the layout. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/144.JPG)

The main thing to focus in the rule is the layer name, which is the layer defined in the special cif output section in the tech file. We can see in the nwell.mag the rule being violated, based on the nwell.6 rule which states the nwell must extend the inside of dnwell by 1.30 microns. The point of the rule is that the edge of the dnwell must be covered with overlap all around by a ring of regular n-well. The outside distance rule casn be implemented by a simple surround drc rule, but the inside distance cant be captured with a simple edge type rule. 

![](https://github.com/YishenKuma/sd_training/blob/main/day17/145.JPG)

We edit the tech file at the style drc section. The way the cifmaxwidth drc rules are implemented with width = 0, implies that the nwell_missing layer is whats leftover, if either the inside or outside dimension of nwell overlap dnwell doesn’t reach the required distance. Evrything in the difoutput drc style is implemented as a temp layer rather than a layer, all temp layers are basically support layers that are needed to get the right results for an output layer, but not appearing in the output themselves. The dnwell_shrink represents the largest open area that you can have inside the drawn dnwell. The nwell_missing layer starts with the dnweel layer, then it grows it by 400, which is the distance required by the surround rule, which gives us the smallest nwell variant that is needed to cover the dnwell.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/146.JPG)

Use the command “cif ostyle drc” because you can only see layers for the cif layer style that is selected for output. Then use the command “cif see dnwell_shrink”, to see that area. Then clear it with “feed clear” and “cif see nwell_missing” which shows the area which gets flagged with the error. 	

</details>

<details><summary> Lab challenge to find missing or incorrect rules and fix them </summary>
	
![](https://github.com/YishenKuma/sd_training/blob/main/day17/147.JPG)

Now we look at the nwell.4 rule, which states that all nwell will contain metal contact in tap, rule checks only for licon ln tap, evry nwell must have an n-tap layer contact, which in magic is called n-contact. Since there is no distance associated with the rule, its impossible to write this as a simple edge based drc rule, but it does lend itself to a cifoutput rule very easily.

![](https://github.com/YishenKuma/sd_training/blob/main/day17/148.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/149.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day17/150.JPG)

The general idea of the rule is to take all ntap contacts and expand and fill the area of any nwell underneath, for that, there is a cif output operator known as bloat-all, after applying the operator, you will have all nwell that contain taps, so all that needs to be done is to take all nwells and remove the set of all nwells that contain taps, and whatever is leftover is an error. 

Read the tech file again and change the style to drc full usiong command “drc style drc(full)” and perform the drc check. 
	
</details>

</details>
	
</details>

## **Day_18: Pre-layout STA And Importance of Good Clock Tree**

<details><summary> Lecture Day 18 </summary>

<details><summary> Timing Delay using delay tables </summary>

<details><summary> Delay Tables </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/1.JPG)

With the use of gates for clock nets, such as shown in the above figure, which is the method known as clock gating, we can ensure no dynamic switching and short circuit power consumed by the clock tree, during the time the clock gets gated.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/2.JPG)

We need to look into the timing characteristics of the buffer, in the case where we want to swap out the buffer for a gate. For each level of buffering, we should have an identical buffer being used, and each node should be driving the same node. We need to keep in mind that the load at the output will be varying, and since the load of one buffer is varying, the input transition of the following buffer will also vary. This means that we will have a variety of delays.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/3.JPG)

The delay table is characterized based on varying the input transition and output load of a cell, against the delay of that cell. Each cell will have its own delay table for different sizes and threshold tables.

</details>

<details><summary> Delay Tables usage </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/4.JPG)

Each type of cell will be having its own individual delay table, as the internal pmos and nmos w/l ratio gets varied, the resistance changes, then RC constant gets varied as well, meaning the delay of each cell gets varied. The values of delay which are not available on the table are extrapolated based on the given data. 

Similarly, to how we have a delay table, we will also have a characterization table for input transition. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/5.JPG)

The latency at the endpoints will be the sum of the delays of each individual cell in that path. The total skew value between two endpoints will be non-zero if the output load driven for a cell is varied, meaning different delay numbers are seen between endpoints, this is why it is preferred to have the nodes at each level driving the same load. Another case in which we can retain the skew to be zero in the presence of varied load, is by using a different buffer size at the same level that can achieve the same level of delay as the other buffer in same level based on its delay table.  

![](https://github.com/YishenKuma/sd_training/blob/main/day18/6.JPG)

These are factors which should be looked into in the early stages of the clock tree design stage. Now we must look into power aware CTS, where we have to consider endpoints which are only active under certain conditions. In these cases, we need not propagate the clock into those cells during the period of inactivity.

</details>

</details>

<details><summary> Timing analysis with ideal clocks using openSTA </summary>

<details><summary> Setup timing analysis and introduction to flip-flop setup time </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/7.JPG)

At the zero time stamp, there is one clock edge that reaches the launch flop. And at the T time stamp, the second rising edge reaches the capture flop. Any analysis that needs to be done is between 0 and T. For the combinational circuit to work, the combinational delay needs to be less than the period, T.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/9.JPG)

Now looking at more practical scenarios. Looking at how the flop works, there will be a delay within the internal flop circuitry, between mux 1 and mux 2. These internal delays will restrict the combinational delay requirements. This internal delay is known as the setup time, and this setup time needs to be subtracted away from the complete clock period T. Now the capture flop has enough time for it to compute the data within the flop and ensure the data is ready at Q by the time the second rise edge of clock reach.

</details>

<details><summary> Clock jitter and uncertainty </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/10.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/11.JPG)

The next practical scenario to take into consideration is jitter. The clock is expected to reach the clock pin at exactly 0s or at Ts, but in real scenarios, the clock signal may not be able to reach at the exact moment, as the clock source generation may have its own built-in variation. This is known as jitter, the temporary variation of the clock period. The combinational delay will become more stringent as a result. Thus we change our combinational delay to factor in the uncertainty factor from the jitter.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/12.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/13.JPG)

The combinational delay of a path will look as shown above. 

The next challenge comes in performing timing analysis with multiple ideal clocks.

</details>

</details>

<details><summary> Clock tree synthesis TritonCTS and signal integrity </summary>

<details><summary> Clock tree routing and buffering using H-tree algorithm</summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/14.JPG)

Clock tree synthesis is done to propagate the clock signals to all the clock pins in the deisgn, however, a good clock tree needs to be designed to take into account the skew between the clock pins due to long routing. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/15.JPG)

Through the use of H-tree, which is a smarter implementation for a clock tree design, which is designed based on the distances between the clock pins in the design between the clock port. This is to give a skew value as close to 0 as possible by having the clock signals reach all the cells at the same time. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/16.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/17.JPG)

The next step is to perform clock tree buffering. The wires for the clock routes each will have resistances and huge number of capacitances, and with the long routing, there will be signal integrity issues, thus, to maintain the signal integrity, we need buffering on these nets.  

</details>

<details><summary> Crosstalk and clock net shielding </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/18.JPG)

Another topic to understand before moving to using real clocks is clock net shielding. Clock nets are the critical nets in the design, we build the clock tree to ensure there is a minimum skew. However, if there is any cross talk that happens and affect the clock signals, that will affect the design very badly. By shielding, we are protecting the clock nets from the outside world, avoiding glitches and delta delays from occurring. If a glitch occurs on the clock net, incorrect data in the memory will cause inaccurate functionality for the design. The shield can be connected to ground or to Vdd, as long as there is no switching activity occurring. Critical data nets are also necessary to be shielded.  

</details>

</details>

<details><summary> Timing analysis with real clocks using openSTA </summary>

<details><summary> Setup timing analysis using real clocks </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/21.JPG)

With real clocks, we will need to have buffers inserted into the clock path to ensure the clock signal integrity. Now because of the buffer introduction, the clock edge will reach the clock pin with consideration to the delays of the buffers inserted. The clock network delay will also need to take into consideration the delays from the buffers inserted. The window will become shifted as a result of the delays from the buffers inserted. The skew for this design will now be the difference between the deltas, and our equation for setup timing analysis will also change based on the image shown above. If the data arrival time is higher than the data required time, then we will have negative slack on the path, meaning we have a violation. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/22.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/23.JPG)

For hold timing analysis, where the capture edge is on the o clock rise edge, the combinational delay should be greater than the hold time of the flop, the hold time refers to the second mux delay, which is the time required for the data to be sent after the clock edge within the flop. So the Data needs to arrive after the hold time, so the new data can be captured into the flop, after existing data is launched out. 

</details>

<details><summary> Hold timing analysis using real clocks </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/24.JPG)

Introducing more real factors into our design for hold analysis will yield the above equation for hold timing. Jitter for the launch clock and capture flop will not need to be taken into consideration as the design is on the 0 clock edge, the arrival difference for the capture and launch flop will be the same, so the uncertainty should be kept low for the hold anlaysis. The slack formula will be data arrival time – data required time, and if data required time is higher, we will have negative slack, meaning the timing path for hold will be violated. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/25.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/26.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/27.JPG)

For the timing path for setup for real clocks, now we need to take into considerations the deltas that were mentioned earlier, for delta1, launch clock network delay, and delta2, capture clock network delay. The equations for setup time and hold time are shown. 

</details>

</details>

</details>

<details><summary> Lab Day 18 </summary>

<details><summary> Timing Delay using delay tables </summary>

<details><summary> Steps to convert grid info to track info </summary>

The next objective in the course is to extract the LEF file, which contains the info on the via boundary, power and ground rates, and the input and outputs, from the .mag file. And, we want to try and plug the lef file into the picorv32a flow, instead of the previous standard cell library. 

There is a guideline that needs to be followed in creating a std cell set. One of the mains ones, is that the input and output ports must lie on the vertical and horizontal tracks. Second, the width of std cell should be based on the track pitch, and the height should be based on the track vertical pitch.  

![](https://github.com/YishenKuma/sd_training/blob/main/day18/101.JPG)

We can see the track info in the lib directory of openland within the pdks folder. Tracks are used during the routing stage. The specifications for the routes for each layer musty be declared before the routing occurs. The ports of the cell are in the li1 layer, so the ports need to be ensured to be on the intersections of the horizontal and vertical tracks. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/102.JPG)

Use the hotkey “g” to activate the grid. Now we can verify if the ports are on the horizontal and vertical intersections of the tracks for li1. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/103.JPG)

We set the grid setting based on the track info as shown above using the command “grid 0.46um 0.34um 0.23um 0.17um”. What we have done is that we have converted the track info into a grid for our cell.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/104.JPG)

Now we can see that the ports are aligned on the intersection for the horizontal and vertical tracks. This ensures that during routing, the routes can reach the ports from both x and y direction. 
 
</details>

<details><summary> Steps to convert magic layout to std cell LEF </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/105.JPG)

Second requirement of guideline for creating the std cell set is that the width and height of the std cell should be in the odd multiples of the x and y pitch of the tracks. 

Whenever a layout is made, the layers are defined, but there are no ports, ports do not mean anything to the validator. Port definitions are required when we want to extract the lef file. The ports will be defined as the pins of the macros. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/107.JPG)

We can use text helper to create the port in our design. The port number refers to the order in which the port is written in the lef file. This is how we define the ports for all the layers in the design. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/108.JPG)

Next, we need to declare the usage of the port, and that is done through set port class and port use attribute for a layout. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/109.JPG)

Once the parameters for the ports have been set, we are ready to extract the lef file. We create the mag file using the command “save <name.mag>”. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/110.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/111.JPG)

Then we open the created mag file and use the command “lef write”, if we do not specify a name, then the lef file name will be based on the .mag file name.

</details>

<details><summary> Timing libs and including new cells in synthesis </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/112.JPG)

We copy the newly written lef file into our design folder for picorv32a. This is so we can include the custom cell into the openlane flow, starting with the synthesis step. We need to ensure the abc step maps the cell appropriately, thus we need to have a library which has the cell definition.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/113.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/114.JPG)

Lastly, we need to modify our config.tcl to ensure the extra lef is read in frm the folder, based on the two commands that need to be run. The -tag and -overwrite options during prep -design is used to take in the new values and overwrite the old values in the runs.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/115.JPG)

During synthesis, we can see the custom cell can be shown to be mapped in. 

</details>

<details><summary> Configuring synthesis settings to fix slack and include vsdinv </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/116.JPG)

In our synthesis we have a worst slack of -24.89, and total negative slack of -759.46. We need to try to find out how we can reduce these values by making the synthesis timing driven, by trying to strike a balance between the delay and the area. Our chip area was reported to be 147712.918400. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/117.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/118.JPG)

The way we can change the strategy for synthesis run is through using the command “set ::env(SYNTH_STRATEGY) “DELAY 3””, instead of the previous value 0, which has more focus on reduced area size. SYNTH_BUFFERING is to insert buffer in high fanout nets, which is enabled by default. SYNTH_SIZING is to perform cell sizing instead of buffering, which is disabled as default, we will enable this. Setting SYNTH driving cell allows us to change the cell driving the port, to use a cell with higher driving power in case we wanted. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/119.JPG)

Now we can see a change from the previous synthesis run, we are having no more slack with a large in increase in size of chip area to 181510.332800.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/120.JPG)

Custom cell exist within merged.lef within temp directory of run folder.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/121.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/122.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/123.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/124.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/125.JPG)

Then we proceed to run floorplan and placement steps. But error is encountered in the run_floorplan flow due to the EXTRA_LEFS variable that was set in the config.tcl causing the flow to stop. The workaqround for this is to comment out the basic_macro_placement command to pass floorplan in /scripts/tcl_commands/floorplan.tcl. And comment out macro placement within scripts/openroad/or_basic_mp.tcl.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/126.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/127.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/128.JPG)

Then we run magic. We can find the custom cell using command getcell. As we can see, the custom cell has been successfully plugged into the custom lane flow.

</details>

</details>

<details><summary> Timing analysis with ideal clocks using openSTA </summary>

<details><summary> Configuring Open STA for post synthesis timing analysis </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/129.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/130.JPG)

Usually what is done in the case that there is a timing violation is that we perform analysis in a separate tool. In our case, we will be using openSTA. We need to write a configuration file as shown above to read in the necessary files. Within the pre_sta.conf, we have a few settings written out for the units, libs and verilog files read, and reports written. We will be reading in the netlist after synthesis stage, as so far we have gone until the placement stage, which has no changes on the netlist. We also need to have written a base_sdc file within the src folder for the sta tool to read. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/131.JPG)

Then we run sta using the command “sta pre_sta.conf”.

</details>

<details><summary> Optimize synthesis to reduce setup violations </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/132.JPG)

For our hold timing, it does not hold any significance as we have not done CTS, and we are assuming ideal clocks, so the slew is zero. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/133.JPG)

For setup timing, we start at the top where our delays are high. The higher the slew or capacitance, the higher the delay of the cell. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/134.JPG)

We will first try to optimize the fanout value. We run synthesis again, but change the value of SYNTH_MAX_FANOUT to 4, from the previous value of 6.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/135.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/133.JPG)

Our value of tns has reduced but not by a large amount, this is due to the high fanout of 33 coming from output net of sky130_fd_sc_hd__dfxtp_2 causing the cap value to be very high. We will tyr to reduce this by upsizing the cell using command “replace_cell _35210_ sky130_fd_sc_hd__dfxtp_4”. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/136.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/137.JPG)

We can now see a reduction in the input transition as well as the delay from the change in the cell type. There is also slight reduction in the wns and tns values. 

</details>

<details><summary> Perform basic timing ECO </summary>

Upsizing the buffer is one of the ways in which we can improve the timing, by increasing the drive strength of the cell while at the sacrifice of size, we improve on the timing. 

</details>

</details>

<details><summary> Clock tree synthesis TritonCTS and signal integrity </summary>

<details><summary> Run CTS using TritonCTS </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/138.JPG)

For openLane to implement the changes we have done in openSTA, we need to use the command “write_verilog” and overwrite the existing verilog file. The we run floorplan and placement, and the new netlist will be read in. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/139.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/140.JPG)

We use the command “run_cts“ based on the parameters set in the config file. The netlist will also be modified as there will be buffers being added into the clock paths. 

</details>

<details><summary> Verify CTS runs </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/141.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/142.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/143.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/144.JPG)

The commands used so far “run_synthesis” “run_cts” are procs within the openlane default settings, taken from the script’s directory. We have a sperate scripts folder for all the open road scripts to be used for the openRoad apps.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/145.JPG)

Clock buffer cells added in the stage. The CTS_MAX_CAP refers to the max cap for the root clock buffer, and this value can be found in the typical lib file that is used for the design within the src folder.

One of the disadvantages of the tritonCTS is that it cannot create an optimized CTS for multi corner, it can also perform for a typical corner. 

</details>

</details>

<details><summary> Timing analysis with real clocks using openSTA </summary>

<details><summary> Analyse timing with real clocks using openSTA </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/146.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/147.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/148.JPG)

OpenRoad has openSTA integrated into the tool. We enter into openroad from the openlane tool using the command “openroad” to perform timing analysis of the clock tree. The benefit of doing this is that we can use the variables set within the openlane flow. Then we need to create a db, based on the LEF and DEF file, using the command “read_lef”, “read_def”, and “write_db”. Then read in the db using “read_db”, and then “read_verilog”, “read_liberty” for max and min, and “read_sdc”. Then use the command “set_propagated_clocks [all_clocks]” to calculate the actual cell delay in the clock path.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/149.JPG)

Timing analysis using command “report_checks -path_delay min_max -format clock_expanded -digits 4”

![](https://github.com/YishenKuma/sd_training/blob/main/day18/150.JPG)

Timing analysis for the hold timing. The hold slack needs to rectified first and foremost as the violation cannot be solved by simply changing the period. 

Once we perform the next stage which is routing, the resistances and capacitances will be introduced will cause the delays to increase further. For hold point of view this can reduce the slack, but will cause the setup slack to become worse. 

</details>

<details><summary> Execute openSTA with right timing libs and CTS assignment </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/151.JPG)

The CTS is built to optimize for the typical corner, but the libraries we have included for this analysis is the min and max libraries, for min and max corners. Thus this analysis is not actually correct. What we need to do is include only the typical library for the typical analysis. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/152.JPG)

Now our timing analysis will be accurate.

![](https://github.com/YishenKuma/sd_training/blob/main/day18/153.JPG)

Timing report for hold analysis. 

Note that both hold and setup timings are now met. For typical corner, CTS would not have any violations. IF we wanted to do for the min and max corners, we would need to do them separately as tritonCTS does not currently support multicorner optimization. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/154.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day18/155.JPG)

One thing to note is that the clock buffers are inserted based on the CTS_CLK_BUFFER_LIST from left to right to meet the skew value, if the skew value is not met, then the next buffer is used, but the buffer will increase in size from left to right. We would want the skew values to be within the 10% of the max clock period. If we wat to use a different clock buffer, we need to remove the clock buffer from the list and rerun CTS. We use the command “lreplace” to remove a value from a variable. 

</details>

<details><summary> Observe impact of bigger CTS buffers on setup and hold timing </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day18/156.JPG)

Now we rerun CTS and recheck the timing reports again. Make sure to change the CURRENT_DEF value back to placement stage, or we will be seeing timing errors, meaning the CTS is not run correctly.  Then enter open road and rewrite the db from the same steps earlier as the db needs to be redone with the new CTS performed. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/157.JPG)

For the hold timing report. The slack values are met but are not improved compare to the previous run even though larger buffers are being used. 

![](https://github.com/YishenKuma/sd_training/blob/main/day18/158.JPG)

Using the command “report_clock_skew -hold” and “report_clock_skew -setup”	

![](https://github.com/YishenKuma/sd_training/blob/main/day18/159.JPG)

If we want to add the buffer type 1 back into the CTS_CLK_BUFFER_LIST, we use the command “linsert”.

</details>

</details>

</details>
	
## **Day_19: Final Steps For RTL2GDS**

<details><summary> Lecture Day 19 </summary>

<details><summary> Routing and design rule check </summary>

<details><summary> Introduction to Maze routing – Lee’s Algorithm </summary>

Routing is the process of creating the physical wire connections within the design. We have algorithms in place top help determine the best way the routing can be done between two endpoints, the source, and the target, with the shortest distance and the least number of zig-zag turns.

![](https://github.com/YishenKuma/sd_training/blob/main/day19/1.JPG)

One such algorithm that we will be looking at is lee’s algorithm, also known as maze routing. The algorithm needs to be aware any blockages set that hinders any routing to be done in a particular area. The first thing that is done in this algorithm is to create a routing grid at the backside of the floorplan. Then two points are created, the source and the target, through the routing grid, the software determines the best route possible through numberings one by one through each possible path to the target, and the path that requires the least number of grids squares to reach the target with least number of turns would be the best route.  

Performing the routing for 1 route will be fairly simple, but when we have millions of start and endpoints to route between, this method will consume a lot of time and memory. There are some algorithms that can help to reduce the time and memory consumption such as line-search algorithm, stanner-tree algorithm. 

</details>

<details><summary> Design Rule Check </summary>

The DRC rules are the rules that should be followed whenever the routing of the design is performed. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/2.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/4.JPG)

One of the rules may be the minimal wire width, where the width of the wire should be no less than a specified amount, based on the limitations of the fabrication process. Another rule that is based on the fabrication process of lithography is the wire pitch, where the centre-to-centre distance between 2 wires should be no smaller than a certain distance. Wire spacing rule, where distance between 2 wires should be no smaller than a certain distance. These are just 3 or the thousand of rule the tool has to adhere when performing the routing of the design. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/6.JPG)

One type of DRC violation is a signal short, where two wires that are not intended to be connected become in contact on the same layer, and this could lead to functional failure, so this needs to be taken care of. We can solve this by simply moving on of the wires on to a different metal layer, but with this, comes new drc rules that need to be adhered to.

![](https://github.com/YishenKuma/sd_training/blob/main/day19/7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/8.JPG)

First is that the via width, where the width of the via should be no less than a certain value. Second is the via spacing, where the distance between 2 vias cannot be less than a specific distance. Most of these DRC rules come from the lithographic process and the limitations that come with the technology. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/9.JPG)

The next step would be to perform parasitic extraction, where the resistances and capacitances of the wires are extracted and used for further processes.



</details>

</details>

<details><summary> Triton Route Features </summary>

<details><summary> Honors pre-processed route guides</summary>

TritonRoute is the tool used to perform initial detail routing. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/10.JPG)

In fast routing, a rough routing draft is created. The fast routing is the engine which is used for global routing. The detailed route is performed by the TritonRoute and the global routing is done by the fast route. During global routing, the region is divided up into grids cells,which acts as a route guide for the TritonRoute to use for the detail routing, where an algorithm is used to find the best connectivity between the points. 

It honours the preprocessed route guides (obtained after fast rourtes), wherein the tool attempts as much as possible to route within route guides. The tool assumes route guides for each net satisfies inter-guide connectivity. Triton route works on proposed MILP (Mixed integer liner programming) -based panel routing scheme with intra-layer parallel and inter-layer sequential routing framework, to finds the best way to perform the routing, where intra-layer refers to the routing within a layer, and inter-layer routing refers to routing between layers, through the uses of vias.

</details>

<details><summary> Inter guide connectivity and intra & inter layer routing </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day19/11.JPG)

The preprocessed guides should have unit width and must be in the preferred direction of the layer. Global route is done by fast route, and the output would be the routing guide. The initial route guides are transformed into the preprocessed guides through splitting, merging, and bridging. Whenever the tool sees the route guide with non-preferred direction, it divides the route guide into unit widths, and then the route with preferred direction is merged, then the non-preferred direction routes is bridged to become a route on another layer, which is the preferred direction for routing. This way, we avoid parallel routing with higher layers, avoiding parallel plate capacitance. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/13.JPG)

Each layer or panel will have its own preferred routing direction assigned to it, in which the routes should be formed. Routing in the higher layers will begin only one the routing the bottom layers have been completed. 

Two guides are connected if they are on the same metal layer with touching edges, or if they are on neighbouring metal layers with a non-zero vertically overlapped area. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/12.JPG)

Each unconnected terminal (i.e., pin of a standard cell instance) should have its pin shape overlapped by a route guide. The purple box in the image would be the routing guide on the metal 1 layer that would overlap with the unconnected terminal. 

</details>

<details><summary> Triton Route to handle connectivity </summary>

The inputs needed for TritonRoute are the LEF file, DEF file, and the Preprocessed route guides. 

The outputs from the TritonRoute would be a detailed routing solution with optimized wire-length and via count.

The constraints needed in using TritonRoute are the route guide honouring, connectivity constraints and design rules. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/14.JPG)

TritonRoute handles connectivity through 2 ways, through either AP, Access Point, or APC, Access Point Cluster. Access pointy is an on-grid point on the metal layer of the route guide, and is used to connect to lower-layer segments, upper-layer segments, pins or IO ports. Access Point Cluster is a union of all Access Points derived from same lower-layer segment, upper-layer guide, a pin or an IO port. The access point refers to the point where the via can be placed to allow connectivity between layers. The objective of the MILP, Mixed Integer Liner Programming is to connect one access point to another optimally. First is to choose one of the access points where the via should be dropped, and second is determining how the first access point will connect to the next access point.

</details>

</details>

</details>

<details><summary> Lab Day 19 </summary>

<details><summary> Power Distribution Network and routing  </summary>

<details><summary> Lab steps to build power distribution network </summary>

If you want to retain the configurations form the last openlane job, you need to use the command “prep -design <design> -tag <tag>”. If you want to create a fresh run with new configurations but without changing the tag name, you need to use the command “prep -design <design> -tag <tag> -overwrite”. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/101.JPG)

Ensure that the current_def is on the CTS stage,  in order to run the power distribution network PDN, before we can perform the routing. We use the proc “gen_pdn” to generate the power distribution network for the design. 
 
![](https://github.com/YishenKuma/sd_training/blob/main/day19/103.JPG)

The LEF files and DEF files are read, then it will create the gird and transfer the power and ground. The standard cells will be placed in the standard cell rows, and for the rows will need to have the power and ground lines along the side rows where the std cells are placed.  Then the straps are provided for the chip. From the power pads, the power goes into the straps, and from the straps, it drills down into the standard cell rails. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/102.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/105.JPG)

Error encountered during “gen_pdn”. Stage cannot move on to perform routing as current_def has not changed to floorplan.pdn.

</details>

<details><summary>  Lab steps from power straps to std cell power </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day19/104.JPG)

The power and ground signals first go into the pads, into the power rings, then through the straps, and lastly, through the rails. 

</details>

<details><summary> Basics of global and detail routing and configure TritonRoute </summary>

To perform the routing, we use the command “run_routing”, ensure that the CURRENT_DEF is set to the floorplan.pdn.def.

![](https://github.com/YishenKuma/sd_training/blob/main/day19/106.JPG)

The variables that can be configured within the routing stage. The routing strategy specifies the optimization mode to be used in TritonRoute. There are 5 routing strategies that can be used in Tritonroute, a value of 0-3 specifies TritonRoute to use engine 30. If the value is set to 14, then TritonRoute 14 will be used. Using the option 0, the default value, means the routing will not be optimal, but there will be a very low runtime and memory consumption. Using TritonRoute 14 may take up to an hour. 

</details>

</details>

<details><summary> Triton Route Features </summary>

<details><summary> Routing topology algorithm and final files list post route </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day19/15.JPG)

Algorithm which is used in optimized routing. For each APC, the algorithm needs to find the cost associated with the distance between 2 APCs, and then a minimum spanning tree, MST, between the APCs and the costs. The objective of the algorithm is basically to find the minimal and most optimal point between the 2 APCs. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/107.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/108.JPG)

Once the routing has completed, we can see the memory that was taken up by the tool and the number of DRC violations in the design port routing. For the run in the image above where the routing strategy was set to 0, less time was taken but resulted in several drc violations. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/109.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/110.JPG)

The fast_route guide is used by the triton_route tool for detail placement to perform the placement within the nets in the route guide. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/111.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/112.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day19/113.JPG)

The next step after routing would be to extract the parasites of the design, and these parasictic analysis need to be done outside openlane,  as they have not yet been integrated. We need to first enter the SPEF_EXTRACTOR dir. To perform the step we also need top declare the LEF and the DEF, and using the command “python3 main.py <lef> <def>”, and this will create the spef file. The SPEF file will be located in the same folder as the DEF file. 

![](https://github.com/YishenKuma/sd_training/blob/main/day19/114.JPG)

As our netlist becomes changed due to the antenna diodes being added into the netlist, our db needs to be rewritten and loaded again with the new verilog file read in for the post_route sta analysis, loaded alongside with the SDC file, and the newly generated SPEF file. We need to check for congestion, timing and then on the DRCs. 

</details>

</details>

</details>

## **Day_20: Floorplanning and power planning labs**

<details><summary> Lecture Day 20 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day20/a1.JPG)

The physical design flow within the RTL2GDS flow involves partitioning the design, chip planning, performing placement and  clock tree synthesis, signal routing and performing timing closure.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/a2.JPG)

Some of the files that are needed within the physical design flow include:

* .tf: technology file, describe the units, layers, design rules, capacitances of the design 

* .lib: reference libraries, contains the cell timing and functionality, for the netlist and design rule constraints

* .gds: graphical data sheet, contains the physical layout information, which is used to create the reference libraries

* .tdf: top design format, contains the pin and port information

* sdc: constraints file, contains timing constraints and clock definitions

* .v: .vhd, contains the connectivity information of the design

The outputs that would be generated from the physical design flow are: 

* .sdf: synopsys design file, generated post floorplan

* .spef: synopsys parasitic ectract format, contains parasitic information

* .v: updated flattened verilog post floorplan and placement

* .hv: hierarchical verilog 

*. gds: contains physical layout information

</details>

<details><summary> Lab Day 20 </summary>

IN order to perform the floorplanning and power planning of  the vsdbabysoc design, we must ensure the synthesis is performed with the relevant constraints applied as well as all the relevant lib files read in. For this we need to clone the necessary github directories https://github.com/Devipriya1921/VSDBabySoC_ICC2.git, “https://github.com/bharath19-gs/synopsys_ICC2flow_130nm” and “https://github.com/bharath19-gs/VSDBabySoC_ICC2.git”.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/2.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/4.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/5.JPG)

Once that is done, we need to open up DC shell to perform synthesis on our design by sourcing the file vsdbabysoc.tcl, with the updated file paths, for all files that is to be used within the tcl file. This will generate the necessary synthesized verilog file, using the command “source vsdbabysoc.tcl”. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20/6.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/6a.JPG)

The next step would be to perform the physical design by sourcing the provided top.tcl script provided, with making the necessary changes to the paths of the local files. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20/7.JPG)

Error encountered in run, no core area and standard cell area set in design, need to review and ensure all correct collaterals sourced

![](https://github.com/YishenKuma/sd_training/blob/main/day20/8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/9.JPG)

Stage error encountered: NDM lib creation, need to ensure correct files are being used for the design
	
Removing references of Nangate and replacing with LEF files of sky130 files, as well as for asvddac and asvdpll.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/10.JPG)

Error still encountered in flow during legalize placement step, no cells being legalized.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/12.JPG)

Cells within design naming not matching with cell naming within top.tcl.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/13.JPG)

Performing legalize placement with appropriate cells still show issue in design, no cells have been placed within design yet.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/14.JPG)

Non fixed macros present in the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/17.JPG)

Macros locations in the design.

Stage error encountered: Placement. wrong file sourced
	
![](https://github.com/YishenKuma/sd_training/blob/main/day20/21.JPG)
	
Stage error encountered: Incorrect files can cause error to occur anyuwhere in deisgm, for this case, it occured during library creation

The LEF file for the design needs to be ensured appropriate for the design, or else the lm_shell will fail during the library creation stage. For this, the LEF file used was obtained from : https://github.com/bharath19-gs/synopsys_ICC2flow_130nm/tree/main/synopsys_skywater_flow_nominal/LEF, for the sky130_v5_7magic.lef, which has fixed on two issues causing error in the flow. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20/x5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/x3.JPG)

We will encounter an error such as this if the LEF file is having issues such as the ones listed below.

> multiple END library definitions were made in the originally used LEF file

> there were multiple definition of the same cells for different versions, in the originally used LEF file
	
Stage error encountered: NDM lib creation

The tech file needs to be appropriately set as well for the sky130 technology, obtained from the directory: https://github.com/bharath19-gs/synopsys_ICC2flow_130nm/tree/main/synopsys_skywater_flow_nominal. The technology file is the most important input for the tool in physical design, as it provides the tech specific information, such as the names and physical and electrical characteristics of each metal/via layers and routing design rule.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/22.JPG)

Within the same directory, we will get the itf file, which is used to generate the tluplus file for the design, that can be used by parasitic extractor in the PnR tool for modelling. The TLUplus models enables accurate RC extraction results by including the effects of width, space, density, and temperature on the resistance coefficients.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/23.JPG)

This may be encountered in the design where no cells get placed, be sure to source in the pns_example.tcl within the flow. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20/24.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/25.JPG)
	
Stage error encountered: Reading Constraints

We need to make a few changes in the top.tcl as well for the placement and legalize_placement to occur successfully. We need top run the legalize_placement command after the create_placement command, as the cells cannot be moved until they are placed, and they are placed during the create placement command. We also need to include the -floorplan option when using the create_placement command to run the design planning styled placement.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/26.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/27.JPG)
	
Stage error encountered: PG creation

We will also need to change some of the layer definitions within the icc2_common_setup.tcl to adhere to the sky130 tech file, as the previous tech file layer definitions were from metal1 -metal10, but for the sky130, we have the naming convention of met1 – met5, so we need to change the parameters so that our run will be free of errors. If the naming convention is not corrected to match the tech file, then the flow will fail during the power grid creation stage. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20/28.JPG)
	
Stage error encountered: Place, CTS and Route

The naming for the filler cells within the top.tcl needs to be corrected as well to reflect the filler cells of sky130 pdk.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/29.JPG)

Flow for top.tcl has successfully completed. 
	
![](https://github.com/YishenKuma/sd_training/blob/main/day20/30.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/31.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/32.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20/34.JPG)

Design shown in the ICC2 gui.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/33.JPG)

We convert the clock object from ideal to propagated using the command “set_propagated_clock [all_clocks]”. And then we can view the timing report for the design with the “report_timing” command.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/35.JPG)

The report for “estimate_timing” was not generated, as there were no estimate timing rules detected on nets.

![](https://github.com/YishenKuma/sd_training/blob/main/day20/36.JPG)
	
Using the command “report_constraints -all_violators -nosplit -verbose -significant_digits 4 > violators.rpt”, we can view all violating paths within the design. 

</details>

<details><summary> Errors encountered during running design stage through sourcing top.tcl for vsdbabysoc using sky130pdk </summary>

<details><summary> standard cell and core area not specified within design</summary>

During floorplanning, incorrect technology file and lef files

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/1.JPG)

Error encountered in run, no core area and standard cell area set in design.

Solution: Remove references of Nangate and replacing with LEF files of sky130 files, as well as for asvddac and asvdpll.

The tech file needs to be appropriately set as well for the sky130 technology, obtained from the directory: https://github.com/bharath19-gs/synopsys_ICC2flow_130nm/tree/main/synopsys_skywater_flow_nominal. The technology file is the most important input for the tool in physical design, as it provides the tech specific information, such as the names and physical and electrical characteristics of each metal/via layers and routing design rule.

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/2.JPG)

</details>

<details><summary> No cells placed within design </summary>

During read_constraints, wrong file sourced, legalize placement after placement of cells, missing option in create placement

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/3.JPG)

Error still encountered in flow during legalize placement step, no cells being legalized. This is because the pns_example.tcl is not sourced correctly. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/4.JPG)

Cells within design naming not matching with cell naming within top.tcl. legalize placement will not occur as naming convention cells are not the same

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/5.JPG)

Non fixed macros present in the design, need to source correct pns_example.tcl.
Solution: source correct pns.tcl, create_placement with -floorplan option, legalize_placemenmt after create_placement. We need to make a few changes in the top.tcl as well for the placement and legalize_placement to occur successfully. We need top run the legalize_placement command after the create_placement command, as the cells cannot be moved until they are placed, and they are placed during the create placement command. We also need to include the -floorplan option when using the create_placement command to run the design planning styled placement.

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/6.JPG)

</details>

<details><summary> Changes needed in the sky130.lef</summary>

During NDM_library_creation, LEF file needs to be correct or the lm shell will not be able to create the required libs for the design. 

We will encounter an error such as this if the LEF file is having issues such as the ones listed below.

> multiple END library definitions were made in the originally used LEF file

> there were multiple definition of the same cells for different versions, in the originally used LEF file

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/8.JPG)

Solution: For this, the LEF file used was obtained from : https://github.com/bharath19-gs/synopsys_ICC2flow_130nm/tree/main/synopsys_skywater_flow_nominal/LEF, for the sky130_v5_7magic.lef.

</details>

<details><summary> Appropriate TLUplus needs to be used for the design </summary>

We cannot use the TLUplus file for Nangate for the design of sky130
Solution: Within the https://github.com/bharath19-gs/synopsys_ICC2flow_130nm/tree/main/synopsys_skywater_flow_nominal directory, we will get the itf file, which is used to generate the tluplus file for the design, that can be used by parasitic extractor in the PnR tool for modelling. The TLUplus models enables accurate RC extraction results by including the effects of width, space, density, and temperature on the resistance coefficients.

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/9.JPG)

</details>

<details><summary> layer declarations within scripts not matching with technology file </summary>

During PG creation

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/10.JPG)

Solution: The scripts used are tailored for the nangate technology file, therefor we need to modify the scripts to match the layer names within the sky130 tech file. The previous tech file layer definitions were from metal1 -metal10, but for the sky130, we have the naming convention of met1 – met5, so we need to change the files having the wrong layer declarations.

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/11.JPG)

</details>

<details><summary> Incorrect filler cell naming</summary>

During place, CTS, and route stage

Solution: change the name of the filler cells that is appropriate to the technology being used

![](https://github.com/YishenKuma/sd_training/blob/main/day20e/12.JPG)

</details>

</details>

## **Day_21: Placement and CTS labs**

<details><summary> Lecture Day 21 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day21/x1.JPG)

PLacement is the process of determining the location of standard cells present in the netlist by placing these cells in the core area. 

PLacement plays a key role as good placemnet of the cells will lead to good routing during the PnR stage. 

The stages in placement include global placement, legailization, and detailed placement. 

> global placement is to generate a rough placement in the core area that may violate some placement constraints, while maintaining a global view of the whole netlist. 

> Legalization, or also known as refine placement, aims to solve the placement violations during global placement by moving moduke to legal loactions on the design, based on the timing, power and congestion.

> Detail placment further improves on the refined placement, by iteratively rearranging a small group of modules in a region while keeping other modules in the other regions fixed. All th fional quality improvements will occur in this stage, congestion, timing and  power need to be taken care of in this stage.

The quality checks or objectives for the placement stage would be to ensure low congestion, high performance, good timing and routability, and fast runtime. 

Clock tree synthesis stage takes in the placement database and CTS specification file, in order to build the clock tree for the design, in order to propagate te clock signals to all the lements in the design that require clcok signal, and ensure minimal difference between he end points in the clock tree.
 
> placement database includes contains the placement completed netlist, def, lef, upf and other files used in the placement database. There will be no more standard cell placemnt on the dabatabase after this point. 

> The CTS spec files hold info on the info on buffers and inverters which are used to balance the clock tree, as well as skew group information, target skew,  maximum target transition, and other timing constraints. There will also be via informatuion to be used for the clock nets routing, as well as rule definitions. 

The steps involbed in the CTS stage inlcude, clustering, DRV fixing, Insertion Delay reduction, power reduction, balancing, and post-conditioning. 

> clustering creates the skew groups based on the spec file

> DRV fixing is to handle design rule violation such as max capacitance, max length, max trabistion, max fanout

> Insertion delay reduction to minimize the insertion delay as much as possible

> power reduction, as clock signals will have a higher consumption

> balancing the the clock nets through clock buffers and inverters

> post conditioning to handle anymore design rule violations found in the design

The quality checks for CTS stage is to check the design skew, pulse width, duty cycle, latency, clock tree powre, signal integrity, and crosstalk. Then we will need to perform timing analysis and fixing. 

</details>

<details><summary> Lab Day 21 </summary>

Once the floorplanning is completed, the constraints and the parasitic files have been read, the placement stage will begin. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l1.JPG)

“plan.place.auto_generate_blockages” option specifies whetehre ti create auto-derived soft placement blockages for the design. These soft blockages are needed so that standard cells do not get added in narrow channels between hard macros. These blockages are usually added after deisgn planning is finished and the block is ready to go to implementation. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l2.JPG)

The create placement command is used to create the coarse placement for the design. The floorplan option runs the design planning styled placement. The placement effort is set to high, and the congestion and timing driven options are used to run timing-driven and congestion-driven placement. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l3.JPG)

Legalize_placement is used to shift the placement of the cells in the design placed during the coarse placement. The design needs to contain a floorplan with a site array specified, as well as all the cells and blockages having an initial placement for the command to be able to run.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l4.JPG)

Placement report generated after the legalize_placement is run, no overlaps, physical hierarchy violations, and no voltage area violations. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l5.JPG)

Next, we have the pin placement for the design, which is done by sourcing the pns.tcl file that was modified in the previous lab to match the current technology file for the power grid creation.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l6.JPG)

Check design for pre-pin placement, having 3 warnings to be reviewed.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l7.JPG)

Preferred port locations that was reported out. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l8.JPG)

Placement for the ports reported.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l9.JPG)

Then we perform the timing estimation for the design. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l10.JPG)

Estimate timing performed.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l11.JPG)

Post estimated timing report for the design shows a violated slack of -0.48.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l12.JPG)

Post estimated timing qor showing 29 violating paths, 368 nets with violations, 364 max trans violations, and 184 max cap violations.

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l13.JPG)

Post estimated timing qor summary. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l14.JPG)

Here we perform the final steps which is placement, CTS and routing.

The “place.coarse.continue_on_missing_scandef” option is set true, checking prior to coarse placement will be disabled, likely because we had performed coarse_placement earlier in the flow. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l15.JPG)

> standard cells placed in the design with names of “{core/CPU_Xreg_value_a4_reg[19][15]} core/U1773 core/U1772 core/U1740 {core/CPU_Xreg_value_a4_reg[19][26]}”

“place_opt” places the current design, performs optimization for the placed design based on timing, electrical drc violations, area, power and routability. It also performs incremental placement to optimize the timing an routability, and finally legalizes the design placements at the end. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l16.JPG)

> clock tree built for design 

“clock_opt” synthesizes and optimizes the clock trees, completes the detail routuing of the clock trees, and then performs optimization based on the timing, electrical drc violations, area, power, and routability based on the actual propagated clock latencies, then finally legalizes the design placement. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l17.JPG)

> routing tracks created on the design 

“route_auto” command is used to run global routing, track assignment, and lastly performs the detail routing, all in one step. In our design, we use a max of 5 iterations for the optimization of the routing, the default value is set to be 40. 

![](https://github.com/YishenKuma/sd_training/blob/main/day21/l18.JPG)

> physical only filler cells added in the design 

“create_stdcell_fillers” command is used to insert the filler cells into the design, filling in the empty spaces in the standard cell rows with instances of filler cells from within the filler cell library specified, in our case is the sky130 filler cells.
	
![](https://github.com/YishenKuma/sd_training/blob/main/day20a/a1.JPG)

Core utilization for design is set to be 7%.

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/a2.JPG)

Utilization ratio of design: 0.27%

</details>

## **Day_22: CTS analysis labs**

<details><summary> Lecture Day 22 </summary>

Clock tree synthesis is method of distrubiting the clock equally among all sequential parts of a VLSI design. And in order to distribute them evenly, we need to ensure that the delays to all the clcok input pins get balanced.

The goal in performing CTS is to minimize the skew and insertion delay. 

![](https://github.com/YishenKuma/sd_training/blob/main/day22/1.jpg)

The cells and objects should all be placed on the design before the CTS stage. Within the CTS stage, we may have Pre-CTS Clock tree power optimization, clock tree syntyhesis, timing optimization, and clock net routing.

The balancing needs to be done as different wire lengths for different paths will incur different delays and skews, and CTS aims to handle this while ensuring good PPA.

![](https://github.com/YishenKuma/sd_training/blob/main/day22/2.JPG)

By typing compile_clock_tree, the main command for the lab, which automatically performs the CTS step. Most of the time the algorithm that would be used is the H-tree CTS or mesh CTS, based on the best choice for the design.

To use multisource CTS would be to take up a lot of power consumption.  

![](https://github.com/YishenKuma/sd_training/blob/main/day22/3.JPG)

In H-tree algorithm, centers of all the flops in the design are found. The tool traces the clock port to the cenetr points. Then the core is divided into 2 parts, in order to tace both parts and reach to each center. Then the center is formed again, abd divided again to trace till teh centers at boty ends. The step is repeated until the clock pins of all the flops are reached. 

There are a number of checks done for the CTS stage, which include,

> skew check

> pulse width check

> duty cycle check

> latency check

> power check

> crosstalk quality check

> delta delay quality check

> glitch quality check
 
The "check_clock_tree" command is used after the CTS stage, this will check the clock tree structure, constraints, and clock tree exceptions that are needed to check in order to have good QOR, quality of results.

"check_legality" should also be done prior to CTS stage, to ensure the placement is done well, and the design is ready for CTS. 

CTS also some default constraints, if there are no user-specified constraints, including max transition, max capacitance, and max fanout. We can edit this using the command "set_clock_tree_options"

We perform clock tree synthesis using the command "clock_opt" which would comprise of synthesizing the clock tree, performing preroute and postroute clock tree optimization.

The command will optimize the design based on the clock tree built, by performing power optimization, re-synthesize teh clcok tree if needed, adjusts i/o timing, performs RC extraction of the clock nets and copmputes accurate clock arrivakl times, and performs placement and timing optimization. 

This command should be run after running teh "compile_clock_tree" command, and running checks, but the command is not existant in the icc2 tool, so we do not run this command.

similaryly to vcs, cts also has a debug mode, which we can use for icc2 by setting the "cts_use_debug_mode" option to true, this allows us to fix issues interactively as we go through the CTS flow

"report_clock_tree" shows the details on the max global skew, late/early insertion delay, number of levels in the clock tree, number of clock tree references (buffers), as well as clock DRC violations

If we have any clock DRC violations, we need to rerun the step and fix these issues, as these cannot be present for the final product.

"report_clock_timing" will show the actual and relevant skew, latency, interclock latencies and other details for the related paths. 

These report checks should be done before and after clock tree optimization. 

We use the command "check_clock_tree -clocks <clks>" to verify that the clock trees are properly defined before the clock trees are syntehsized. 

</details>

<details><summary> Lab Day 22 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x1.JPG)

The checks to be performed were added into the top.tcl before and after the CTS stage for checking the quality of CTS and verifying readiness of design for CTS.

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x2.JPG)

Firstly is to check legality, before the CTS is performed, to ensure the placement is done well and design is ready for CTS. 

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x4.JPG)

Ensure legalize_placement command is already run prior to check_legality, or else run check will fail.

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x3.JPG)

Check_clock_tree showing 1 warning CTS-904 for pll cell not having LEQ cell specified. Pending to check.

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x6.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day22/x8.JPG)

“report_clock_timing -type {interclock_skew/latency/skew/transition/summary}” for the design

</details>

## **Day_23: Clock Gating Technique and Routing**

<details><summary> Lecture Day 23 </summary>

### Clock gating

When we perform clock tree synthesis, we also need to be taken into the consideration of the power consumption, especially in designs with a large number of clocks, meaning that in the synthesizing of a clock tree, there will be a greater number of buffers in the design, inducing a larger area, and also a larger power usage. 

One way to be able to handle the complexity of task of building the clock tree for the entire design is by, partitioning the design into smaller parts, and performing the clock tree synthesis individually for the clocks, and then in the family level, have a fully completed routed tree. 

![](https://github.com/YishenKuma/sd_training/blob/main/day23/1.JPG)

Partitioning of the design is done, and then later the buffers for the clock tree will be inserted.

We need to not only keep in mind area and timing, but we also need to beware the power factor when doing CTS, for designs with high number of inverters or buffers.

One way that we can perform power aware CTS is through the clock gating technique using AND, OR and universal NAND gates. These cells are used to gate the clock in order to save power. One thing to note, is that 50% of dynamic power was found to be lost from clock related circuits. Our design may have unnecessary power usage on the clock circuits, even if it is not being used all the time, the switching activity of clocks that take up power may not be used by the design for some instances. This is why clock gating is a useful technique for power handling, as the clocks are gated when they are not used by the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day23/2.JPG)

From the diagram, we can understand that the functional unit will only take in the CLK as an input based on the clock gate, which is dependant on the EN feed by the activation action, Fcg.

Clock gating in an industry standard will be done at the synthesis stage, and then optimized in the implementation stage (physical design).

### Routing

After CTS is performed, we need to ensure that there is a physical connection between all the signal pins in the design through the use of the metal layers, this is known as routing.

There are three types of routing, which include P/G routing, Clock Routing, and Signal Routing. 

![](https://github.com/YishenKuma/sd_training/blob/main/day23/3.JPG)

> P/G routing

![](https://github.com/YishenKuma/sd_training/blob/main/day23/4.JPG)

> clock routing

![](https://github.com/YishenKuma/sd_training/blob/main/day23/5.JPG)

> signal routing, including global and detailed routing

</details>
	
## **Day_24: Timing violations and ECO**

<details><summary> Lecture Day 24 </summary>

ECO stands for Engineering Change Order, which are essentially last minute changes for the design to fix any issues found, instead of fixing them at the start and rerunning the flow, which would take too much time and resources.

The RTL code will be modified for a small change to fix issues seen at the end, and these changes will need to pass all the verifications before it can be passed to layout. This ECO will need to pass the formal and functional verification before the layout can be edited. The implementation of the ECO in the layout should fix and seal all the sign-off checks that were not done during the physical design flow. Make sure the ECO does not incur any new issues in the design as well.

There are various strategies in designing an ECO. The steps in implementing an ECO are, firstly, investigating the problem using the latest database, then, generating the ECO to address the problem. Third, implement the ECO on the latest database. Lastly, save the database for future, once the implementation is done and problem is fixed. The strategies for ECO include:

> Margin Based Fixing (DRV, max trans, max cap, setup and hold violations)

> Selective endpoint biased fixing (with and without margin/ slack range)

> slack based fixing (setup/hold target slack, max slack)

> fix ‘n’ number paths (number of paths per group(max_paths)/ endpoint(nworst))

> GBA, group based, and PBA, paths based, fixing

> Full chip vs reg2reg fixing

> leakage fixing using HVT

> Hierarchical ECO (top level/ individual/ replicated hierarchies/ all)

> physical aware ECO (routing congestion aware, cell legalization, buffer on route)

</details>

<details><summary> Lab Day 24 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/2.JPG)

Constraints for design is read in before placement is performed. We need to modify the constrains such that the “set_clock_latency” does not get applied. We run remove this in place and route flow only, the verilog netlist remains the same.

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/5.JPG)

The timing report that will be generated will be using ideal clocks for the analysis. Our post estimated timing pre-CTS report is slightly improved but is still violated.

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/4.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/6.JPG)
 
![](https://github.com/YishenKuma/sd_training/blob/main/day20a/10.JPG)

Once CTS stage is completed, we need to convert the ideal clocks into propagated clocks, it should be ideal only for post placement timing analysis. Once we rerun the flow, we can observe the changes on the timing paths of the design. Now from our timing report post CTS, we can see that the timing for the design has not been improved, with the changes on the remove_clock_latency constraints. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/11.JPG)
 
![](https://github.com/YishenKuma/sd_training/blob/main/day20a/12.JPG)

Fanout constraint not set on design, sdc file needs to be reviewed to optimize design. As a result path is having paths with high fanouts 

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/7.JPG)

One way we can do this is by upsizing the cells based on the post timing report based on the analysis column. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/13.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/17.JPG)

We will try to optimize the path “-from core/CPU_is_add_a3_reg -to core/CPU_Xreg_value_a4_reg[27][31]” based on the analysis shown in the post estimated timing report pre CTS stage. 

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/14.JPG)

The timing slack has been improved but still violated for the path after the eco change is implemented.

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/15.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20a/16.JPG)

We can see from our QOR comparison before and after the eco step, there is an increase in combinational area, as well as an increase in hold violations. But there is a reduction in max trans and max cap violations.

</details>

<details><summary> Day 25 update: Adding decap cells into design </summary>
	
Decap cells can help to reduce IR drop or reduce noise in mixed signal designs
temporary capacitors added in the design between power and ground rails to counter functional failures due to dynamic IR drop

![](https://github.com/YishenKuma/sd_training/blob/main/day20j/j1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20j/j2.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day20j/j4.JPG)

Decap lib cells to be inserted into design, based on modification in top.tcl

![](https://github.com/YishenKuma/sd_training/blob/main/day20j/j3.JPG)

> power report before decap cells added

![](https://github.com/YishenKuma/sd_training/blob/main/day20j/j5.JPG)

> power report before decap cells added, reduction in cell internal power, increase in net switching power

</details>

## **Day_26: Introduction to mixed-signal flow**

<details><summary> Lecture Day 26 </summary>

The most available signal available in nature are analog signals, but a microcontroller or microprocessor will understand or speak based on signals that are either 0’s or 1’s, which are digital signals. In order to allow these microprocessors or microcontrollers to take in analog signals into the design, we need to use ADCs and DACs. The conversion process of and ADC or DAC needs to perform well in order to be able to get a precise number, we will always end up with an offset error which is not healthy for the calculation. The conversion process includes 3 steps, which are, sampling, quantization and encoding. 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/0.JPG)

> https://www.javatpoint.com/difference-between-analog-signals-and-digital-signals

Analog signals will be more precise, but will have more noise, whereas, digital will have less noise and easier to read, but will have less accuracy and more error content.

We need mixed signal chips to replace the use of bulkier ADCs and DACs in applications, which is able to measure signals with high precision. Mixed signal chips are able to atleast partially deal with input signals whose precise value matter, which includes RF, Analog, Analog to Digital and Digital to Analog conversion. These chips will have a very different design and process and technology demands than normal digital circuits. 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/1.JPG)

In AMS design flow, there are 2 paths, the analog blocks an digital blocks. The analog and digital blocks go through similar but different paths but end up at mixed signal analysis after simulation is performed. Then the digital and analog blocks undergo similar processes of physical layout and verifications, before processing for full chip assembly and physical verification, and then mixed signal functional verification. 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/2.JPG)

The diagram above shows how an analog signal is converted into a digital signal through the use of an ADC block, and also how that signal is converted into an analog signal through the use of a DAC block.
 
In the previous VSDBabySOC deisgn that we have worked on, we were having three blocks in the deisgn, the blocks are as follows

* RVMYTH processor -digital

* PLL – analog

* DAC – analog

### Collaterals in design flow

The most important files that are needed in creating designs include:

* LEF file – library exchance format, holds physical properties regarding cells

* LIBerty file – contain timing information of cells

* gdsII and OASIS file -  contains the whole chip design in a format that enables layout design to be transferred from one place to another, to be viewed or used for verifications 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/3.JPG)

All the collaterals used in the PnR tool to create the gdsII file. 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/4.JPG)

Summarized description of the physical design flow.

![](https://github.com/YishenKuma/sd_training/blob/main/day26/5.JPG)

Source of the files needed for the collaterals of physical design flow.

### IP cores

Ip cores consist of a block of logic or data used in a semiconductor chip. Intellectual property core, is used to make filed-programmable gate array (FPGA) or application specific integrated circuit for a product. They are created throughout the design process and can be turned into components for reuse. IP cores have 2 types , hard (has logic and physical implementation, the physical layout of a hard macro IP is fixed and finished) and soft (can be customized during physical design phase and mapped to any other process technology). 

![](https://github.com/YishenKuma/sd_training/blob/main/day26/6.JPG)

The diagram above shows how it works in the semiconductor industry, which is heavily affected by moore’s law, wherein the size of a transistor is predicted to reduce in size by half every 2 years. This comes with newer and more challenges to overcome.

</details>

## **Day_27: Introduction to crosstalk – glitch and delta delay**

<details><summary> Lecture Day 27 </summary>

In the VLSI design, there may be times when the nets that are routed are getting impacted by the noise from other nets, the capability of a net to overcome the noise from other signals and carry uncorrupted values is known as signal integrity. A design has good signal integrity if if tuis able to carry information reliably and resist the effects of the high-frequency electromagnetic interference from nearby signals. 

Crosstalk refers to a type of noise signal that corrupts the actual signal while transmnitting, usually between two or more adjacent nets due to capacitive cross coupling.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/1.JPG)

> https://www.vlsi4freshers.com/2020/04/crosstalk-and-noise.html

The victim net refers to a net that receives undesirable cross-coupling effects from nearby net/nets.

The aggressor nets refer to the net that would cause those effects on the victim net. The aggressor net is also susceptible to becoming a victim net as well. 

In order to ensure successful tapeout of the design, we need to perform the quality checks for the signal integrity and the crosstalk.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/2.JPG)

> https://medium.com/@einfochips/crosstalk-analysis-and-its-impact-on-timing-in-7nm-technology-abcfb795190f 

Crosstalk glitches refer to spikes on nets during its constant state, caused by the switching activity occurring on a nearby net, causing the coupling capacitance to occur between the 2 nets. 

</details>

<details><summary> Lab Day 27 </summary>

In order to perform crosstalk delay analysis, we need to enable the primetime SI through the app_var “si_enable_analysis” to true.

Second is to back annotate the design with cross-coupling capacitance information in a SPEF or GPD file. This is done through the command “read_parasistics -keep_capacitive_coupling file_name.spf”. For this, we need to generate the spef file from our icc2 shell with our design loaded. For up-to-date parasitics, it is recommended to do update_timing before write_parasitics.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a2.JPG)

Once we have all the necessary input files for PT_shell, we need to load the design to begin the analysis.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a4.JPG)

> set link_library                [list  /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsddac.db /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/mew/VSDBabySoC/src/lib/avsdpll.db]

> read_verilog -design vsdbabysoc/init_dp -top vsdbabysoc /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/rvmyth/report/vsdbabysoc_gtlvl.v

> link_design vsdbabysoc 

> read_sdc /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/rvmyth/report/vsdbabysoc.sdc

> set_app_var si_enable_analysis true

> read_parasitics -keep_capacitive_coupling /nfs/site/disks/png_mip_gen6p9ddr_0042/ymaniraj/rvmyth/vsdbabysoc_spef.temp1_25.spef

We use the check_timing command, and commands for checking specific to crosstalk analysis: 

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a6.JPG)

> check_timing is unsuccessful, warning shows that are 5 ports with parasitics but having no driving cells. Warning also prompt showing check unable to compute the rising/falling RC network delay from 1 pin to another.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a9.JPG)

PT_shell gui shows no endpoints for the analysis types for the vsdbabysoc design.

Then we will have the timing reports, and the bottleneck reports to analyze. 

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a8.JPG)

> report_timing -crosstalk_delta, path timing from cells are not shown in the path, as compared to timing report done in icc2_shell.

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a11.JPG)

> report_si_bottleneck

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a10.JPG)

> report_bottleneck

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a12.JPG)

> report_si_double_switching

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a13.JPG)

> report_noise

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a14.JPG)

> report_timing -transition_time -crosstalk_delta \ -input_pins -significant_digits 4

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a13.JPG)

Some of the repair strategies that can be used for the nets reported out in the bottleneck reports include using the commands: 

> size_cell

> set_coupling_separation

> minimum_active_aggressor

The corsstalk net delay can be done using the command:

> report_delay_calculation -crosstalk \ -from [get_pins g1/Z] -to [get_pins g2/A]

We can check on the crosstalk settings through the commands:

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a15.JPG)

> report_si_delay_analysis

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a16.JPG)

> report_si_noise_analysis

![](https://github.com/YishenKuma/sd_training/blob/main/day27/a17.JPG)

> report_si_aggressor_exclusion
	
Design does not seem to be loaded correctly, pending debug.

</details>

## **Day_28: Introduction to DRC/LVS**

<details><summary> Lecture Day 28 </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/1.jpg)

Physical verification checks the correctness of the generated layout design, through the four steps, which are DRC, LVS, ARC, and ERC.

> DRC: design rule check, determines if the layout satisfies a set of rules required for manufacturing.

> LVS: Layout versus Schematic, verifying that the layout created is functionally the same as the schematic/netlist of the design.

> ARC: antenna rule check, checks for possible issues in layour design that may lead to plasma induced fate oxide damage during manufacturing, also known as antenna effect

> ERC: electrical rule check, checks design for all electrical connections that are considered dangerous.

</details>

<details><summary> VSDIAT Day 28 </summary>

<details><summary> Day 1: Introduction to skywater sky 130 </summary>

<details><summary> Introduction to SkyWater PDKs and opensource EDA tools </summary>

<details><summary> Introduction to Skywater PDK </summary>

PDK stands for Process design kit, it is a bundle of files and documentation needed by the designer to know how to work with the process foundry an use it to make chips. 


![](https://github.com/YishenKuma/sd_training/blob/main/day28/4.JPG)

130 in the sky130 refers to the feature size, referring to the length of the smallest transistor that can be made in the process. 

Skywater refers to the manufacturer.

Skywater pdk is mainly comprised of the documentation and the PDK library and files, as well as community.

Documentation: https://skywater-pdk.readthedocs.io/en/main/ 

PDK library and files: https://github.com/google/skywater-pdk 

Community: https://invite.skywater.tools/ 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/2.JPG)

> Information on the sky130 pdk can be obtained here: https://github.com/google/skywater-pdk 

The SkyWater Open Source PDK is a collaboration between Google and SkyWater Technology Foundry to provide a fully open source Process Design Kit and related resources, which can be used to create manufacturable designs at SkyWater’s facility.

The SKY130 is a mature 180nm-130nm hybrid technology originally developed internally by Cypress Semiconductor before being spun out into SkyWater Technology and made accessible to general industry.

The SkyWater Open Source PDK documentation can be found at https://skywater-pdk.rtfd.io. 

The skywater pdk works with efabless.com to get their custom boards for free provided that the users design must be made available in 	a public repository.  

![](https://github.com/YishenKuma/sd_training/blob/main/day28/3.JPG)

> https://efabless.com/

</details>

<details><summary> OpenSource EDA tools </summary>

The tools working with the skywater pdk include: 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/5.JPG)

* Open_pdks: works with any process in theory, with any other open process descriptions, so it is now mainly an installer for the skywater 130 process.

> http://opencircuitdesign.com/open_pdks/

> https://github.com/RTimothyEdwards/open_pdks 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/6.JPG)

> open pdks work through the following steps above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/7.JPG)

The magic tool is the backbone of the openPDKs installer and is mandatory to have installed before running the make file. Magic performs extraction and DRC, and can create design layout form parameterized descriptions either within the layout tool or within the schematic. Magic is responsible for creating any file format for any cells that is missing from the repository sources.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/8.JPG)

Klayout is an alternative layout  editor and viewer and can also do DRC.  Openpdks will install a skywater sky130 compatible setup  file and script to do the DRC checks. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/9.JPG)

Openlane is the synthesis and route package based on the open road tools, it's basically a wrapper around the open road tools with various setups and scripts that support the skywater process.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/10.JPG)

Xscheme is a schematic editing tool. It is not directly implemented in openpdks,  but it's a third party repository that openpdks can pull in and copy it to its common installation location.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/11.JPG)

Netgen is the LVS tool that typically works with a netlist extracted from a layout using magic, and the netlist generated from Xscheme or from openlane. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/12.JPG)

Ngspice is the analog simulation tool based on Berkeley spice and openPDK is installed all the model files such that Ngspice can find them with the right include statements.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/13.JPG)

There are a few other alternative tools including qflow, an alternative digital synthesis flow, IRSIM, a switch level simulator and power analyzer and Xcircuit, an alternative schematic entry and schematic capture tool. Additional tools can be added to open PDK either as built-in entries like magic and open lane or a third party entries like Xscheme. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/15.JPG)

In addition to the tool setups for open source EDA tools, openpdks will install the foundry and third party libraries, creating a directory structure common across all libraries regardless of the source, that's the main goal of openpdks, to have a common file system structure and method so that all EDA tools can automatically know where to find all the libraries files and information that they need. This is especially important for open source tools because they are spread around maintained by different groups and not fully integrated. There are upsides to this, but the downside is that methods can get very fractured and incompatible if there isn't a common framework that everyone agrees to work with.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/14.JPG)

> SkyWater SKY130 Installed Filesystem Structure

![](https://github.com/YishenKuma/sd_training/blob/main/day28/16.JPG)

> Open PDKs Project Filesystem Structure

</details>

<details><summary> Understanding Skywater PDK layers </summary>

The skywater sky130 process is described as a hybrid 130 nanometer 180 nanometer standard CMOS fabrication process. Mostly fet transistors have a minimum length of 150 nanometers, though specifically designed memory layouts use 130 nanometer long devices.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/17.JPG)

There are five layers of aluminum metal plus a layer of titanium nitride which is used like a metal layer but is relatively high resistance, so it is not good for long routes. This layer which is called local interconnect, Li, is the most nonintuitive layer in the whole process for anyone used to process this where the first layer of metal above polysilicon is an aluminum routing layer. The general rule for using local interconnect is to use it to connect neighboring devices but otherwise contact up immediately to the metal one. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/18.JPG)

In the skywater standard cell layouts, the local interconnect is used for the power and ground rails , but it should never be used for routing the entire length of both rails of local interconnects strapped with metal one above them. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/19.JPG)

Contacts to polysilicon require a nitride Poly cut layer around the contacts, usually this isn't an issue but it is possible to place contacts in ways that seem legitimate but cannot satisfy the design rules for the nitride polycot layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/20.JPG)

The metal layers are in a progressive thicknesses with local interconnect being the thinnest followed by metals 1 and 2 and then a thicker metal 3 and 4 and finally a thick metal 5, which is a bare minimum of metal layers for this feature size. When running digital flows the tool should reserve metal 5 for routing and with local interconnect unusable for routing there are only metals 1 through 4 to route with. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/21.JPG)

Metal layers and vias are called the back end layers and everything below that is called the front end there are often distinctly separate with different precision required for the masks and of course different fabrication steps. They share the steps of oxide growth, but the front end is mainly diffusion and ion implantation while the back end is mainly metal deposition. 

On the front end, the main difference in use of layers for the skywater process vs other processes is that they have divided the diffusion layers into diff and tap layers, where diff represents the heavily doped regions used transistor source and drain while tap represents the oppositely doped region used for well and substrate contacts. Most silicon fabrication processes do not distinguish between these two since they're both fabricated with a diffusion method in the same step and they're only differentiated through different doping levels, there are implant masks for these different doping levels so the information needed to distinguish a source or drain region from a tap region is already available. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/22.JPG)

Other useful front end layers to know about are the deep N well, which is an N well buried so deeply that there's room to diffuse P well region into the area above it. The deep N well layer then creates a barrier N-doped region sandwiched between the P substrate and the P well. The isolated region allows P type devices such as fet transistors, bipolars and diodes to be completely isolated from the substrate, this isolation comes at the expense of the area required for surrounding the whole deep N well region with an N well ring to completely isolate the P well region on all sides, and the large required spacing between the separate deep N wells of multiple isolated domains are needed. However, the improvement in noise isolation is worth those drawbacks 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/23.JPG)

The HVI layer is a high voltage implant which has more than one use. Firstly, N well implanted with HIV is tolerant to higher voltage levels, the mask is also used to grow additional insulation under the gates of mosfet transistors forming what is known as a thick oxide gate transistor. The thick oxide devices are tolerant of voltages up to around 5 volts and the skywater process while the nominal thin oxide devices are only tolerant voltages up to about 2 volts. This leads to typical dual voltage domain designs which analog circuits are designed with thick oxide devices and run at a common voltage of 3.3 or 5 volts, and core digital circuits are made in the thin oxide devices and run into voltage of 1.8 volts. The pad frame cells and the skywater IO library reflect this dual domain design methodology with a typical core voltage of 1.8 volts and a pad voltage of 3.3 volts. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/24.JPG)

The MIM cap layers are part of the back end process, although they form devices that are extracted and simulated from a design standpoint, they feel more like part of the front end. MIM stands for metal insulator metal and these capacitors are formed by adding metal plates between two metal routing layers. The skywater process is notable for having the dual MIM process, in which capacitors can be fabricated between metal layers 3 and 4, but also between metal layers 4 and 5, making a stacked capacitor with double the capacity of one layer only. The capacitors are particularly useful because by being fabricated up in the back end layers the area underneath them remains available for placing transistors and other front end components.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/25.JPG)

There is one other metal layer made available in the skywater process, which is called the redistribution layer and it is not fabricated by skywater, but is fabricated by a third party manufacturer specializing in the process. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/26.JPG)

Redistribution layers are typically used to form bump bonds, a part of WLCSP packaging which stands for wafer level chip scale packaging. The redistribution metal layer which is copper is deposited on top of the finished chip and solder bumps are added on top of the redistribution metal. The end result is that the die itself becomes its own packaging, no wire bonding is needed, the chip is just flipped upside down and soldered directly to a circuit board with the reflow process. The redistribution layer is usually not a design layer and is considered more as part of the chip packaging. However, the copper layers are thick compared to the underlying process back end more than four 4  thick, and can be useful for forming conductors on the top of the chip. In any case, analog miners have to be aware of any redistribution layers on top of the design and in addition that the chip is flipped with circuit board power and ground planes directly underneath

</details>

<details><summary> Understanding Skywater PDK devices </summary>

Understanding the devices is important for physical verification since much of the physical verification is concerned with correctly identifying and extracting all devices on a chip. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/27.JPG)

Like most larger feature size processes that are good for analog and mixed signal design, the skywater process has numerous device offerings for resistors, bipolar devices, capacitors, etc. The best bipolar devices are vertical bipolars, making use of the NP junctions between diffusion regions and wells. Processes like these skywater 130 nanometer process that have deep N well layers can have properly isolated in NPN transistors with the N layers being an N diffusion layer for the emitter, a P well for the base and the deep N well as the collector. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/28.JPG)

PNP bipolars are limited in use is the only configuration requires that the collector be grounded as it is tied directly to the substrate. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/29.JPG)

The best resistors are made with doped polysilicon. There are two specialty devices in the skywater process, one of these is a P+ doped Poly resistor with sheet resistance of around 1 kilogram per square and there is a P- doped Poly resistor with a sheet resistance of around 2 kilograms per square.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/30.JPG)

For some applications, diffusion resistors are appropriate, but since they have a PN junction underneath they must be used in circuit design specifically to keep the junction firmly reverse biased. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/31.JPG)
The highest resistance per square is the P well resistor, but due to the large size and spacing requirements for the P well layer, it is rarely a practical choice especially when high sheet resistance Poly resistors are available in the process. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/32.JPG)

One oddity of the skyward process is that most devices have a discrete set of sizes that have valid corresponding models, meaning devices aren't characterized across a continuous change in width and length. For a number of the devices using a device size that is not one of the valid characterized sizes is not even allowed, the precision resistors for one come in five discrete widths that correspond to a layout around an integer number of contacts. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/33.JPG)

Devices with a restricted number of approved layouts are not all that uncommon in process PDKs, typically a number of devices are carefully laid out and thoroughly tested and that layout becomes the single reference design. Those devices are passed on to the user by the foundry GDS files and the user is expected to use those layouts as is without touching them. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/34.JPG)

There are a number of mask layers that are specific to a handful of devices with fixed layouts, because of that most players really don't need to be shown to the designer. Most such layers are identifier layers, such as the capacitor or resistor or bipolar identifiers which need to cover the device but have no design rules associated with them other than they need to cover the extent of the device. The designer would not even need to know that an identifier layer is there.

</details>

<details><summary> Understanding Skywater PDK libraries </summary>

The skywater openPDK is distributed along with a number of complete IP libraries from the foundry. The library should contain everything that the user needs to work with that IP. There are three types of libraries immediately available in the skyward PDK: digital standards libraries, IO cells, and primitive devices. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/35.JPG)

The digital standard cell libraries all come with layout of every cell and GDS form and files that are normally used by digital synthesis flows such as liberty, timing files, lef technology files and abstract cell views, verilog descriptions of the cells, and spice CDL netlist. There are various flavors of digital cells seven of them and all covering a range of uses from low power to high speed, high density, high voltage, and low leakage. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/36.JPG)

The libraries all follow a standard naming convention, and all cell names and device names contain the library name as a prefix. The library names are in the form of the sky 130_vendor_library-type, and then optionally an abbreviation for the library, if there is more than one library per type. So the most commonly used the digital library, the high density standard cell set is named sky 130_FD_SC_HD. The library name prefixes all of the standard cells, so the standard cell name may be for example sky130_FD_SC_HD__nor2_2, “__” used as the separator between the library name and the cell type. Typically it's the synthesis tools that worry about what drive strength to use not the user.  

![](https://github.com/YishenKuma/sd_training/blob/main/day28/37.JPG)

For the design using digital standard cells in a schematic, be aware that the standard cells are designed specifically to be placed in a row, so any manual layout containing standard cells should treat them the same way placing them next to each other according to the bounding box, and not overlapping or spaced apart.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/38.JPG)

Another important library is the IO cell library. The skywater 130 nanometer process has a particularly complicated set of io cells that are legacy of a series of chips designed by cyber semiconductor. They have a number of unusual features and many of those features are not going to be of interest to most designers. The efabless harnessed chip design exists as a good reference on how to put together a pad frame with these cells. The name of the IO library is sky 130_FD_IO.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/39.JPG)

One problem with the IO library from skywater is that it contains power and ground pads which have entire disconnected blocks in them. One example of what is expected is that the Vdd IO pad cell would be connected to the Vdd IO ring going around the pad frame, but there is an overlay cell that is needed to connect the Vdd IO pad to the Vdd IO bus. There is also an ESD voltage clamp in the same cell but it's not connected to any power domain, so if you want the Vdd IO Pad to connect to the Vdd IO ring and also have VDD IO power clamp for ESD protection, there's supposed to be another overlay cell for that, only those overlays don't exist. Fortunately the openPDK installer takes care of those problems by supplementing the IO library with a set of cells that include the missing overlays and other cells which conveniently combine the base cells and the overlays together. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/40.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/41.JPG)

The primitive device library which is named sky 130_FD_PR contains devices that have very specific layouts that are approved by the vendor, which in this case is the foundry. Those layouts include regular transistors with layouts that are optimized by best practice design for RF or radio frequency use, that generally means carefully controlling the parasitics to avoid signal attenuation or noise through parasitic channels.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/42.JPG)

Other specific device layouts in the primitive library can include bipolar transistors, high voltage drain extended devices, ESD devices and large array of parallel plate capacitors of all shape sizes and metal layers. It is not advised to use the parallel plate capacitor simply because there are MIM caps available which have much higher capacitance per unit area without picking up all the routing area above a design. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/43.JPG)

There are two libraries that have not been distributed with skywater PDK which are the SRAM and NVRAM libraries. The SRAM library has been handed over to the open RAM project. The original sources from the foundry included only the core SRAM cell layout and so the open ramp project is creating the additional cells needed for the decoding and driver circuitry, eventually these cells will be put together in a library and either added to the skyward PK or just left as a third party library. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/44.JPG)

There is less of an offering from skywater for the NVRAM which is to say nonvolatile ram such as flash eprom. What is there is not much more than just the design rules for the floating gate Sonos transistor. An NVRAM library would need not only the same basic decoding and driving circuits as an SRAM library, but it needs additional circuitry for the high voltage charge bumps and circuits to control the programming and erasing.

</details>

<details><summary> Opensource tools and flows </summary>

The file formats that are posted are specifically chosen for the ability to be open sourced which are non-proprietary formats and so they should be able to be used with open source tools. EDA tools whether commercial or open source or not really known for their variety of offerings but there are a handful to choose from.

First to design the circuit and make sure it works, we need to know what tools can be used to do the design and do a functional verification and do a physical. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/45.JPG)

We will use a tool called Xschem to create the schematic. Xschem is well integrated with both ngspice and gaw to design and functionally verify a working analog circuit.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/46.JPG)

The schematic is something that can be used to generate a netlist, and the netlist can be simulated with Ngspice. The same netlist and spice format has all the information needed to know what the devices should look like in the layout. For the layout we'll use the tool magic.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/47.JPG)

The PDK is written so that the device drawing procedures can be kept in a file and sourced at the time the program starts. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/48.JPG)

Each device requires a set of routines to describe. It each device is heavily parameterized so that the way the device is drawn depends on the way the parameters are given to it.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/49.JPG)

Some of these parameters are the same parameters that you have control of in the schematic drawing program. Some parameters are very layout specific and don't appear in the schematic such as where to put contacts or whether to add a guard ring and whether to contact ends up to a routing layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/50.JPG)

The starting point and creating layout is straightforward, export a schematic to a netlist, then you import that netlist into the layout.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/52.JPG)

The next step in the manual flow will be to move the devices around in the layout until they pass DRC checks and then wire them together. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/53.JPG)

The final step will be to run LVS again. LVS takes a number of forms but in this case, the traditional one is performed, which is comparing a layout to schematic. They need to be compared as spice netlist formats. 

From the schematic side, a netlist will already be generated for simulation, we use that same netlist imported into the layout tool to see the layout. We use a method called extraction which built into the layout tool. We'll issue a set of commands to the layout tool and from that, we get a second netlist that describes the circuit as the layout tool sees it.

The layout tool has to look at the actual mask layers and the layout and decide for itself how those layers interact to form devices with no prompting and ideally no additional information above and beyond the actual mask layers in the layout. 

Now we have 2 netlists, one is the schematic that is drawn to symbols and the other is a layout drawn with mask layer geometry. Run the LVS tool which compares these two netlists and tells us whether or not they are equal to each other. If they are not equal, then the design needs to be debugged until the design is matching.  

</details>

</details>

<details><summary> Tool installations and basic DRC/LVS design flow </summary>

<details><summary> Check tool installations </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x1.JPG)

Running magic with Gui and console

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x5.JPG)

Running magic without console

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x7.JPG)

Running magic without console or gui

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x2.JPG)

Running Netgen

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x9.JPG)

Running Netgen with Gui, not recommended as has high memory consumption

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x6.JPG)

Running netgen without console

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x3.JPG)

Running Xschem

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x4.JPG)

Running ngspice

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x8.JPG)

Running test script on magic, netgen and xschem tools

</details>

<details><summary> Creating Sky130 device layout in magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x10.JPG)

Setup required before creating sky130 device, copying the links makes it easier to run instead of remembering the command lines.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x11.JPG)

Running xschem

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x12.JPG)

Type E to open a design, and CTRL e to close a design

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x13.JPG)

Loading magic with sky130 technology loaded

> using the command “magic -d XR”, allows us to load magic but with more rendering of the graphics

> with the command “magic -d OGL”, allows to load and use a faster version of magic tool

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x14.JPG)

Paint on layers on the design by selecting desired area and hovering over the substrate, then hit the middle key on the mouse to apply the layer. Use the e command to erase layer. Hover over the tool bar to see the layer names.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x15.JPG)

Create a device by drop down devices 1

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x16.JPG)

The device can be modified by change the settings on the param window and hitting apply. Get description of selected “s” material by typing “what” on console

</details>

<details><summary> Creating simple schematic in Xschem </summary>

Load xschem and click new schematic under file

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x17.JPG)

Click the insert key on keyboard to choose a symbol in the device.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x18.JPG)

Selecting an nfet from the sky130_fd_pr library

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x21.JPG)

Insert the ipin, opin, and io pins for the device, then wire up the whole device.

> m: move

> del key: delete

> c: copy

> q: properties

Change the name and properties of the pins and fets as well.

It is best not to use any specific power supply pins, since there is no concept of a global supply pin or net in a layout. Tere could be issues in verifying the layout if not adhered to.

Change in number of fingers in the fet device also means we need to change the width to be changed, as the original width is only for one finger.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x22.JPG)

Save the design as inverter.sch

</details>

<details><summary> Creating symbol and exploring schematic in Xschem </summary>

We want to have a testbench that is separate from the schematic itself, this is a best practice to functionally validate the circuit. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x24.JPG)

Create the symbol by drop down bar Symbol, and select create symbol from schematic. Then start a a testbench schematic by clicking file and, clicking new schematic. Insert the created symbol in the local directory.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x25.JPG)

Get the default power supplies from the xschem library. Connect two voltage sources, one to the input, and one to the power rail. Make the connections to the ground node. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x26.JPG)

To create the proper spice testbench, we need to generate a ramp input to be able to view the output response. We do this by changing the voltages for the voltage sources to the values shown above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x27.JPG)

We need to include two box statements for ngspice, it is not specific to any components but need to be included in 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x28.JPG)

Click on netlist to generate the netlist, then on simulate to get the simulation waveform for the inverter layout. Now we can see that the functionality of the inverter has been verified. We can then proceed to create a layout for it. We need to edit the device again, we can click e to do this. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x29.JPG)

Under simulation, click the LVS betlist option, then create the netlist by clicking the netlist button.

</details>

<details><summary> Importing schematic to layout and inverter layout steps </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x30.JPG)

Open the spice netlist for the inverter through import spice. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x31.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x32.JPG)

The device is not laid out as we need to do this ourselves. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x33.JPG)

The parameter table can be show for a device by selecting and typing ctrl p.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x34.JPG)

Arrange the pins accordingly for the inverter layout.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x35.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x36.JPG)

Modify the fets parameters, to put a local interconnect, and split the local interconnects to the top and bottom fets. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x37.JPG)

Wiring up the design.

</details>

<details><summary> Final DRC/LVS checks and post layout simulations </summary>

Save the layout.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x38.JPG)

Perform extraction using the above commands. First command ensures extractions go to local directory, second command performs the extraction. Setup the netlist generator for hierarchical output ngspice format,  and then create the spice netlist.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x39.JPG)

Clean up the additional files created in the directory using the command shown above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x40.JPG)

Running netgen “netgen -batch lvs” shows that the netlist circuits match uniquely. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x41.JPG)

In order to perform extraction with parasitics, we need to use the commands above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x42.JPG)

The output spice netlist shows all the parasitics extracted for the design. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/x44.JPG)

If we run ngspice with the layout extracted netlist, we can see that the 2 netlist are verified to be functionally equivalent. 

</details>

</details>

</details>

<details><summary> Day 2: DRC/LVS Theory and labs </summary>

<details><summary> Introduction to DRC and LVS </summary>

</details>

<details><summary> Understanding GDS Format </summary>

Design analysis and simulation are the underpinnings of all chip design. Physical verification however is the protective barrier between the designer and design failure. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b1.JPG)

Design rule checking make sure that the entire design layout meets all silicon foundry rules for mass making. 

Layout versus schematic make sure that the design layout electrically matches the design as implemented in schematic form or any form which is an electrical description of the circuit that is independent of the layout. For LVS only two sources are used an compared to.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b2.JPG)

In modern practice, the tendency toward automation means that chips are designed from a single source usually a register transfer language RTL like verilog or VHDL. The process of LVS is the matter of checking the entire design flow through different routes, one starting at the RTL source and working forwards and the other starting at the finished layout and working backwards.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b3.JPG)

Wherever a tool exists that can do physical verification it should be applied, as it adds robustness to the process.  

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b4.JPG)

CIF was a popular layout file format, it had 2nice properties, which was that it was in human readable asking format and that it was naturally extensible. 

One downside of the CIF format was that any rectangle with an odd integer width can have its center point on an off grid position. The center point is not a physical point so it doesn't have to lie on a grid point, but the corners do have to lie up on grid points. To accommodate that all output concept is scaled up by two times inside each cell to account for the off grid rectangle centers.  

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b5.JPG)

CALMA later introduced the GDS stream format , which is now the preferred format for the mask making. Magci software uses the GDS format now as well.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b6.JPG)

We can see this in the use of cif see command in magic.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b7.JPG)

The layer purpose pairs is what really distinguishes gds format. Every layer in the layout is described not by name but by two numbers, one to denote a layer like diffusion Poly or metal one and another to denote a purpose like drawing label

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b8.JPG)

So GDSII is called a stream format, meaning you can output it all in one go from end to end. The output is in small self-contained packets or something but it's no more or less streaming than any other format. 
The biggest disadvantage of GDS format is that it isn't binary with lots of null bytes and commands and the unprintable end of the ASCII set so you can't see anything in a file without either reading it into a layout editor or using a program to convert it into ASCII.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b9.JPG)

Every file format to describe chip data needs to encode the same basic things, data are in the form of rectangles are polygons, and have a layer associated with them. The formats keep strong sense of hierarchy and you can collect geometry together and call it a cell and you can make instances of that cell and put them in other cells possibly rotated or flipped.We want to preserve some layout metadata which includes stuff that isn't part of a physical mask like labels, cell names, and instance names. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b10.JPG)

There are a few additional tools in the openpdks repository under the common directory. These scripts are for replacing cell names and place within a file, or changing time stamps.

Oasis is a new format which is supposed to produce much smaller output files than GDS. It does that but at the expense of taking out the last bit of readability and GDS files and making the whole thing completely comprehensible. Fortunately it can just be treated as a filter convert your files into Oasis to save space and convert it back when you need to.

<details><summary> Extraction Commands, styles, and options in magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b11.JPG)

Chip layout file formats don't contain much metadata and that includes any concept of a netlist that corresponds to the layout. We need for the layout tool to be able to independently generate the circuit netlist equivalent by looking at nothing other than the mask geometry of the layout. This is a process known as extraction.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b12.JPG)

In the magic layout editor extraction is a straightforward process. It is a two step process in which magic generates an intermediate format of its own devising called the .ext. The second part is to gather the .ext format data and produce a netlist in a known format like spice.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b13.JPG)

There is one .ext file inumerates all the devices like transistors capacitors and resistors used in the layout and all instances of cells that are used within that cell, all of the common connections from the cell down to the sub cells and all parasitic capacitances between nets and from nets to other nets.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b14.JPG)

This is enough to build a complete netlist, and with a spice netlist you can run a spice simulator, or you can pass the netlist along with a schematic capture netlist to compare the two.


![](https://github.com/YishenKuma/sd_training/blob/main/day28/b15.JPG)

The main commands to extract in that list from a circuit are shown above.

extract do local ensure all all the dot EXE files are written locally instead of in the same place as the dot mag layout file from which they were derived.

extract all does the main work of extracting each cell into a dot EXT well and for a large circuit like a full chip it can take a long time

ext2spice LVS is an option set up, there are a lot of possible options, but with this option produces the kind of output that you want to have for running LVS. If you choose the LVS option then the output is automatically in a format that is syntactically correct for ngspice.

ext2spice does the work of converting the TXT files into a single .spice netlist

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b16.JPG)

To simulate a netlist you need a testbench netlist. You'll need to supply your circuit with all the necessary stimuli as well such as power supply and input voltages. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b17.JPG)

you'll need include statemenst at the top of the file to point to model files because the layout editor doesn't know anything about device models. All files that contain device models and parameters for the devices and the circuit need to be included. Since the test bench is a wrapper around the actual circuit netlist, you'll need an include line that includes the netlist that the layout editor generated.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b18.JPG)

Finally you'll need some kind of analysis control block telling the circuit what analysis to run. Then we can run ngspice to perform functional verification.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b19.JPG)
the technology file generated in the magic directory is divided up into a number of sections each corresponding to 1 aspect of the layout tool such as the DRC engine the GPS generator the GS reader the extractor and others. 

Each section can come in any number of varieties called styles, each style begins with the keyword style and the name for the style and it ends with the start of another style or with the end of the section. The styles exist to do different things and each one has a purpose. To select a style, you wriute extract style “style”. The difference in the style variance that's the way that magic generates the output.

</details>

<details><summary> Advanced extraction options in magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b21.JPG)

Additional extraction options 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b22.JPG)

Ext2spice LVS runs with the above options

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b23.JPG)

Extracting with capacitance

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b24.JPG)

Extracting full RC

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b25.JPG)

All commands for rc extraction

For command references in magic, we can learn more on them here: http://opencircuitdesign.com/magic/ 

</details>

<details><summary> GDS reading option in Magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b26.JPG)

Commands for reading gds can be found here

> gds read file 

> gds readonly true|false

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b27.JPG)

Some cases the vendor files have layers that cannot be represented correctly, if the cells come from vendor we cannot make changes to them. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b28.JPG)

Use of readonly option

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b29.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b30.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b31.JPG)

Use of lef files in design and abstract view

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b32.JPG)

Difficulty in reading gds if hiearachy is split

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b33.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b34.JPG)

Flatten options to solve issue

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b35.JPG)

No duplicates option to ignore cell memory

</details>

<details><summary> GDS writing, input, output styles and output issues </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b36.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b37.JPG)

Writing options for gds

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b38.JPG)

Merge option to turn everything into polygons

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b39.JPG)

> best to use the vendor cif style when reading vendor files. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b40.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b41.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b42.JPG)

Ensure using correct input or output styles before reading or writing.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b43.JPG)

Gds output issues

</details>

<details><summary> DRC rules in magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b44.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b45.JPG)

Magic drc interactive engine. There is higher lag with more intensive drc rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b46.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b47.JPG)

Different ways to perform DRC checking, default is fast, more intensive is to use full

Main DRC rule checking with style fast checks edge based rules and Boolean geometry rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b50.JPG)

Use of cifmaxwidth for rule checking

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b48.JPG)

Abstract views is a good way to perform drc checks on some cells

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b49.JPG)

Errors in a cell can be resolved in the hierarchy above it

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b50.JPG)

</details>

<details><summary> Extraction rules and errors in magic </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b51.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b52.JPG)

Extract section of magic tech file includes layer heights and thickness. Tech file will contain the parasitic capacitances.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b53.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b54.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b55.JPG)

Extraction errors in magic

</details>

<details><summary> LVS setup for netgen </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b56.JPG)

Netgen used for lvs

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b57.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b58.JPG)

It becomes more complicated if subcircuits are used, when reading spice files. Technology setup file for lvs tells tool what the device names are, how the connections would be, if there is a need for combination, and which properties to compare between netlists. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b59.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b60.JPG)

Lvs setup for netgen

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b61.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b62.JPG)

How lvs handles hierarchy

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b63.JPG)

Cascading mismatch issue

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b64.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b65.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b66.JPG)

Lvs for layout against verilog

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b67.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b68.JPG)

Black boxing in lvs, you cannot run lvs down to the transistor level, all logic gates will be black boxed

</details>

<details><summary> Verification by XOR </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b69.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b70.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/b71.JPG)

We can perform verification through XOR file generation in magic, compares the layout to see the differences in layouts. Verify no unintended masks were changed.

</details>

</details>

<details><summary> Labs for GDS read/write, extraction, DRC, LVS and XOR setup </summary>

<details><summary> GDS Read </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y2.JPG)

Read in the gds file based on the full path

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y3.JPG)

we can find all the cells loaded through the cell manager, under the options tab

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y4.JPG)

Here we have loaded the and2_1 cell into the gui.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y1.JPG)

The commands above shows the ways we can check the istyles available and the istyle being used. The istyle currently being used is the sky130(vendor). The ports are treated as ports.
 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y6.JPG)

If we change the istyle to sky130(), and read the gds file again, the layers in the layout view has been marked yellop, meaning thy are treated as regular text. It is better to be using the vendor style when dealing with vendor files.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y9.JPG)

If we don’t want to overwrite the existing cells when reading gds, we set the gds noduplicates option to true, now when we change the style and reread the design, it will not update the cell.

</details>

<details><summary> Ports </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y10.JPG)

If we select on a port, and type port index, we can tell the index for that port.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y11.JPG)

This can only be done for 1 port selected at a time.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y12.JPG)

The gds format is not great as it does not preserve most metadata. As we can see from tgeh port queries above, the values are set to default for the port definitions.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y13.JPG)

If we look at the and2_1 subcircuit definition in the library folder, sky130_fd_sc_hd.spice, the cell definition is listed above. Even though the cell definition in the netlist shows A, the gds read in file shows first port as VPWR. The correct port order that should be considered is the definition form the vendor. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y14.JPG)

In order to add this metadata into the gds file in magic is to read the corresponding lef file.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y15.JPG)

Now, we see that the port class and use has been updated by the lef file. But the port order has not been updated. Magic has no spice read command to to provide the layout information. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y16.JPG)

The way we can get the port order from the spice file is using the command shown above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y17.JPG)

Now we can see the port name has also been updated as per the spice netlist.

</details>

<details><summary> Abstract views </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y18.JPG)

IF we read in only the lef file without the gds file, we will see the abstract view of the cell.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y20.JPG)

We can see the port order metadata is also not shown accordingly, however the use and class has been set appropriately.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y22.JPG)

We will need to perform the same readspice command to update this. And reload the cell form the cell manager. Now the naming for port is fixed as well.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y23.JPG)

If we try to create a new layout and instantiate the cell using getcell command, this will load an abstract view of the cell. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y24.JPG)

 Writing this lef file with the above command will prompt the error message above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y25.JPG)

Reading the written gds file, we will see the above layout. This si because magic should not be writing abstraction views to gds. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y27.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y28.JPG)

If we use the command “save test” instead, and load that, we will get the appropriate cell view loaded from the magic file.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y29.JPG)

Since we did save instead of write, the cell that was being edited was the cell that was saved, and not any subcells. The standard cell contents being edited was from the path above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y30.JPG)

If we now try the gds write command, there would be no warning and we would have a valid gds file. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y31.JPG)

We can make the cell writeable using the command above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y32.JPG)

If we paint over a layer of Li over the cell, and write it to a gds, then the new gds file would remain unchanged, as the previous design was still a form of abstraction.

</details>

<details><summary> Basic extraction </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y33.JPG)

To perform extraction of the loaded design, we use the command above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y34.JPG)

We will have the generated spice file as shown above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y35.JPG)

If we use the ext2pice lvs and cthresh 0 options, before running ext2spice, we will have the above spice netlist as shown above with the parasitic cpacitances shown with the lines starting with C.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y36.JPG)

If we rerun again but with the value of 0.01 for the cthresh value, we will have less lines of parasitics written.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y37.JPG)

In order to run a full RC extraction, we need to use the commands above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y38.JPG)

We will see the number of nets that are found usable. The tolerance is a threshold for determining when a network needs to be replaced by a resistance network. Now we will have a .res.ext file that holds information that can be modified for R parasistics. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y39.JPG)

Extract the netlist using the commands above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y40.JPG)

We will now have a spice netlist containing both the R and C parasitic components.

</details>

<details><summary> Setup for DRC </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y41.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y42.JPG)

By running the python file as shown above, we will run a full DRC check on the design and export the results into a txt file.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y43.JPG)

There are different ways DRC checks can be run, the default style is drc(fast). 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y44.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y55.JPG)

If we change the style to full, the drc violations in the design will be shown as seen above. Typing why will show the explanation for the violation.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y45.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y46.JPG)

We can solve all these drc violations by simply adding a tap cell to the design, and aligning it to the right of the and cell. If we look into the and cell, we can see the errors present, but on the top level layout, these errors will not be seen. This is how the hierarchical drc check works for magic. 

</details>

<details><summary> Setup for LVS </summary>

Create the netgen directory for running the lvs check for the design, and copy the necessary files to run netgen as done previously. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y47.JPG)

Reopen magic. We had already created the .ext file, but we need to setup for lvs using the commands above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y48.JPG)

Run the LVS check using the command above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y49.JPG)

We can see that the lvs check is done and that the netlists are matching uniquely.

</details>

<details><summary> Setup for XOR </summary>

We can also run XOR verification in order to see the changes made to a design.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y56.JPG)

Load the same and cell in magic, but save the design as a secondary cell to be altered.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y51.JPG)

Erase a small amount of the LI layer from the design, amd flatten the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y52.JPG)

We run the XOR comparison firstly by generating an xor magic file.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/y53.JPG)

Then we can see the difference between the altered design and the original design through the xor magic file.

</details>

</details>

</details>

<details><summary> Day 3: Front end and back end drc </summary>

<details><summary> Introduction to DRC rules </summary>

<details><summary> Introduction to basic silicon manufacturing process </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c2.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c3.JPG)

Fabrication planar process through layer masking. Mask is needed in lithography step for creating patterns, usied in etch or implantation.

The reason why moore’s law proves true is because each generation, the machines used to create masks improve. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c4.JPG)

Limitations due to fabrication issues.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c6.JPG)

Goal of design rule to avoid failure in fabrication

Rules need to be passed before it can be accepted by a manufacturer

Process yield in manufacturing is the percentage of working devices in a batch

</details>

<details><summary> Backend metal layer rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c9.JPG)

Minimal width rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c11.JPG)

Minimal width rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c12.JPG)

Wide spacing rule

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c13.JPG)

Notch rule

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c14.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c15.JPG)

Max min area rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c16.JPG)

Min hole rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c17.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c18.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c20.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c21.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c22.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c23.JPG)

Via rules

</details>

<details><summary> Local interconnect rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c24.JPG)

Comparison between layers that can be used as wires for connections.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c25.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c26.JPG)

Local interconnect should be treated like polysilicon, not to be routed with. Only used to connect neighbouring circuits, not as long haul routing

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c27.JPG)

For any device terminal, they should be connected up to metal layer 1 through local interconnect directly

</details>

<details><summary> front end rules, transistors implants, ID and boundary layers, wells, and same net rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c28.JPG)

Front end rules affect all devices such as transistors and resistors

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c29.JPG)

PDK includes automatic parameterized device generator in magic to draw complete device that satisfies all rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c30.JPG)

Devices in magic, some devices cannot simply be drawn by hand

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c31.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c32.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c33.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c34.JPG)

Rules related to layer masks

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c35.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c36.JPG)

Types of devices defined by implant layers

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c37.JPG)

Use of locked layers

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c38.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c39.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c40.JPG)

Wells needs to connect with a tap to set the bias voltage

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c41.JPG)

</details>

<details><summary> Deep N-well and high voltage rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c42.JPG)

Isolating an area using an nwell to provide noise isolation

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c43.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c44.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c45.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c46.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c47.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c48.JPG)

Rules for deep n well 

</details>

<details><summary> Device rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c51.JPG)

Resistors can be very complicated thus have many rules associated

Capacitors include 4 types which are varctors, MOScaop, vertical parallel plate (VPP) and Metal insulator metal (MiM).

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c52.JPG)

Rules for varactors

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c53.JPG)

Rules for MOScap

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c54.JPG)

Rules for VPP

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c55.JPG)

There aren’t many reasons to use MIM

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c56.JPG)

Rules associated for MiM

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c57.JPG)

Diodes formed using ID layers, which don’t have drc rules, follow the rules for diffusion tap and well.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/c58.JPG)

Fixed layout devices

</details>

<details><summary> Miscellaneous Rules latch up antenna stress rules </summary>

Some miscellaneous DRC rules are not particularly layer specific, they are presented in the process documentation under the x category

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g2.JPG)

Off grid rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g3.JPG)

Angle limitations

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g4.JPG)

Seal ring rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g6.JPG)

Latchup rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g9.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g10.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g12.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g13.JPG)

Antenna rules

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g14.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/g15.JPG)

Stress rules

</details>

<details><summary> Density rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o1.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o2.JPG)

Any deviation on flatness on layer will affect the upper layers above it. Physical polishing is needed to level out the layers. Chip has to have a certain amount of flatness. Metal wires are like bumps on the chip, the best way to minimize the bumpiness is to ensure surfaces uniformly covered by metal all over. This is what is meant by density rule. Ideal metal density falls around 60%. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o3.JPG)

There are automated tools to create fill patterns. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o4.JPG)

Analog designers hate patterns because they introduce extra capacitances all across circuit that is difficult to analyse. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o5.JPG)

There are occasions fill generations do not meet necessary density.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/o6.JPG)

Placing metal in extremely high density can cause failure as well.

</details>

<details><summary> Recommendation rules, manufacturing rules and ERC rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/h1.JPG)

It is good to follow the recommended rules to improve device robust.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/h2.JPG)

Recommended rules define difference between test chip and production chip.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/h3.JPG)

Rule violation in the final design require a waiver.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/h4.JPG)

Electrical rule checks, ERC are checks for layouts that are DRC clean but may cause circuit failure due to electrical problems.

</details>

</details>

<details><summary> Labs for all DRC rules </summary>

<details><summary> Lab or width rule and spacing rule </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z1.JPG)

Clone all the necessary file from the github link shown above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z2.JPG)

We will begin with excersice 1 for width rule, spacing rule, wide spacing rule and notch rule.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z3.JPG)

For the width rule, it is stated for metal 2 that the minimum width required for the design should be no less that 0.14um. If this is not adhered to, it can lead to spot defects, causing open circuits. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z4.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z6.JPG)

We can fix this by either painting the metal 2 layer to the appropriate amount, or by stretching the existing layer.

We can perform strecting by selecvting over an area, clicking a, and move the area using the numpad keys while holding shift.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z8.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z9.JPG)

The spacing rule gives the minimum required spacing between 2 layers. If we do not fix this, it can cause material defect, leading to shorts. Solve this my moving the layers apart.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z10.JPG)

We can do this also by selecting the region, typing the semicolon key, and typing the commands above.

</details>

<details><summary> Lab for wide spacing rule and notch rule </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z12.JPG)

For the wide spacing rule, if a wire or piece of layout is wider that a specified distance, then the other wires must set apart from it by a specific amount of space. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z13.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z14.JPG)

For the notch rule, we need to give the minimum space between two forks of the same layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z16.JPG)

Now we can see that all drc violations have been resolved.

</details>

<details><summary> lab for via size, multiple vias, via overlap and autogenerate vias </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z17.JPG)

Moving on to rules related to vias.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z18.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z19.JPG)

The size of a via needs to be large enough by a certain amount. We can fix this by simply stretching the via. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z20.JPG)

In order to see how vias are created in magic, we need to look at the second example. Placing the cursor around the contact and checking the cif format layer names. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z21.JPG)

The contacts between layer 1 and local interconnect is known as MCON. IF we run cif see MCON, we can see the MCON for the second example showing multiple vias. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z22.JPG)

Run command above to remove the MCON cuts.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z23.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z24.JPG)

In the first example, if we had not resized the design, the MCON cut would not be bale to fit, and the via could not be placed there.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z25.JPG)

Similarly if we stretch the design further, we can see multiple vias can now be added into the design.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z26.JPG)

In this example, we have an overlap error being shown

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z27.JPG)

We need to have a layer of metal 1 surrounding the box by 0.03um.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z28.JPG)

We also need to have the metal overlap of 0.06 in one direction based on the rule, using the stretch tool we can fix this.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z29.JPG)

If we want to auto generate via without the use of boc manipulation, we can use the keyboard shortcuts. Hitting the spacebar key will switch the cursor type, and then we can use the cursor used for drawing wires. BY holding down shift and left clicking, we can drop a via to the top layer. To drop a via to the lower layer, we need to hold shift and right click.

</details>

<details><summary> Lab for minimum area rule and minimum hole rule </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z30.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z31.JPG)

For this, we are having a metal area that is not meeting the minimum area rule, to fix this simply stretch and increase the area. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z32.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z33.JPG)

Here we have a minimum hole rule violation. Magic does not show this error unless we set the style to full. To fix this, we need to erase the sections until the hole size meets the requirements of 0.07um2. 

</details>

<details><summary> Lab for wells and deep N-well </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z34.JPG)

In this example, we are having errors on our well layers because there is no taps inserted on the design. N-well will show the error as it is floating, but we will not see the error on the P-well as the process does not consider them, unless they are deep p-wells, which then will be treated as p-substrates.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z35.JPG)

We need to paint on a layer of nsubstratediff, which does not fix the error yet. The n well cannot be floating, so we need to also have a layer of local interconnect. Add the layer of nsubstratecontact which will get rid of the drc violations. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z36.JPG)

To fix the errors seen, we need to fix the drc violations by stretching the design adequately, and as mentioned, adding the local interconnect. Once this is done, there will no longer be any drc errors. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z37.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z38.JPG)

We do the same for the pwell, adding in the psusbtratediff, then the psubstratecontact, and lastly adjusting the design to fix the remaining drc violation, as well as the layer of local interconnect.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z39.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z59.JPG)

Here, the drc violation faced is shown above for the deep nwell.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z40.JPG)

First we stretch the area out such that the area of the deep n well increases.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z41.JPG)

We alse need to move the design away from the design in example 4b, as there seems to be a rule violation form the distance between.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z42.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z43.JPG)


We need to then add an n-well overlap around the deep n well area. We can do this using the wire tool as well.

Lastly, we simply need to add in the n-tap as was done before.

</details>

<details><summary> Lab for deprived layers </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z44.JPG)

Here we have the derived layers, we can check to see what are the overlapping layer that is considered, this can be done using what command, which shows us that this is an nmoslvt layer. If we try recreating this as seen below, with the ndiff and poly layers, we see that this area is not considered nmoslvt but as simply nmos. This is because of the specifications in the tech file. If we want to get a layer of nmoslvt, we need to paint in the layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z47.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z60.JPG)

In order to understand the implant layers, we will be using the above commands. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z49.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z61.JPG)

We can also see the implant lvt layer on the nmoslvt using the commands above. The difference between the nmoslvt and the nmos we created.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z50.JPG)

What shows us the layers in this example. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z51.JPG)

This is a high voltage nmos, thus there should be a high voltage implant, HVI. We can verify this using the command above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z52.JPG)

The HVI is slightly bigger than the NSDM implant layer. The high voltage implant does not cover the tap contact however, since the substrate will be grounded, thus it will not see the high voltage. There is however, a high voltage tap which can be painted over the existing tap. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z54.JPG)

We can see the HVI implant which covers the tap if we look at the implant layer

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z53.JPG)

If we add a layer of ndiff above as shown, we will get the following drc error. This si because ethe HVI layer must be kept a certain distance away from the regular low voltage layers.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z55.JPG)

Poly contacts also need a special layer etch instead of implant, called nitride ploc cut, NPC. This layer etches through any nitride residues on the poly to ensure firmer contact between the LI and the poly.

The NPC layer must also bridge between two contacts to avoid any spacing rule errors

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z56.JPG)

There needs to be an additional geometry generated for the contacts of all NPC layers to satisfy all width and spacing rules. These additional geometry may overlap the diff layers, but will not violate the design rules.

</details>

<details><summary> Lab for parameterized and PDK devices </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z57.JPG)

Here we have an nmos device, which is a magic generated device, but still shows drc errors. The error is a minimum area rule error. Magic could avoid the error by adding more metal to the layer, but does not as these contact will be routed to and have metal then.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/z58.JPG)

If we simply paint over metal 1 over the contacts we will no longer see these errors.
	
![](https://github.com/YishenKuma/sd_training/blob/main/day28/e1.JPG)

For the next example, we have an esdfet designed to be able to survive high voltages. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e2.JPG)

The drc violations in the design is due to having transistor gates at an angel which should not be used

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e3.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e4.JPG)

The way that can be done for magic to ignore rules that should be good is by av=bstracting it. All library views are somewhat abstract, they contain pointers to gds files, thus what is shown is nothing more than magic tools attempt to represent the gds data.

We could change the layout without altering what is written to gds, which is usually only used for read only files that don’t get affected. We can use this to make the layout drc clean while not flagging false positives.

We change the path of the cell to our local directory. Then confirm the pointer to gds file is still valid.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e5.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e6.JPG)

Begin clearing off the drc errors by selecting and erasing the angled poly sections until all the drc errors have been reduced to zero.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e7.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e8.JPG)

We do the same for 6c, which is to save to our local directory and perform the same changes to implement the fixes.

</details>

<details><summary> Lab For Angle Error And Overlap Rule</summary>

Magic tool has a grid setup following the manufacturing grid that is provided. Magic can scal up the grid by a factor of 2, making the smallest possible box size 0.01um x 0.01um.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e9.JPG)

If we try to scale down the magic internal grid with the command above, magic will prompt an error message saying that this is prohibited.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e10.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e11.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e12.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e13.JPG)

If we try to create a triangle polygon and overlap it with a flipped copy, magic will try to legalize the overlap as seen above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e14.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e15.JPG)

In exercise 7a, the triangle polygon was created into a subcell, then the copy was flipped and overlapped. This will avoid magic from compensating by legalizing the overlap, we will still get the drc error stating, position dows not align with manufacturing grid. We just need to fix this by selecting one of the shapes and moving them apart.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e16.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e17.JPG)

Here we have the error that 90 degree angles are only permitted on local interconnect. To fix this we simply need to paint over the angled edge with more LI.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e18.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e19.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e20.JPG)

Here we have another angle error but not on LI, if we click to see the box size we see that it is not a proper 45 degree due to the 201 x 200. To fix this, we repiant the angle, and fix the small drc violation by painting in more metal1 layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e21.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e22.JPG)

For this overlap error, we do not se the nmos created similar to past. This is because the poly and diff layers are in different cells. Magic does not create the overlap because of this. To fix this we just repaint the layer of poly, which will create the nmos as seen.
 
![](https://github.com/YishenKuma/sd_training/blob/main/day28/e23.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e24.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e25.JPG)

Overlaps in contacts are having different rules. Contacts have to overlap exactly to adhere to auto generation rules. In this example, the overlap cur has been pushed over to align properly. 

Diving into one of the layers, we can see the contact cuts aligned correctly, and in the top level, they are rearranged to error free, but have the overlap drc violating.

We fix this by flattening the design, this is seen on the copy on the right. Both contacts are on the same layer and have no concern for overlap. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e26.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e28.JPG)

Here we have via contacts not aligned correctly.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e29.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e30.JPG)

To fix these, we need tom simply adjust the position until the contacts align exactly.

</details>

<details><summary> Lab For Unimplemented Rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e31.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e32.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e33.JPG)

In this exercise, we have a seal ring. Seal rings are layers that have no electrical meaning. They simply exist as a physical barrier between the chip and the outside world. 

We see that the seal ring is breaking design rules. Magic only shows these seal rings as an abstract view to be drc clean, having not associated properties. We will get overlap errors if we try painting on a diffusion layer.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e34.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e35.JPG)

We will use the seal ring generator from the skywater pdk to generate a gds that has correct seal rings, these cannot be imported however unless as abstract views.

To generate the seal rings, we only need to specify the size of the pad frame outer edge.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e36.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e37.JPG)

This will create a .mag and .gds.  using the addpath and load commands, we will see that there is now a references for the gds during the property command. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e38.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e39.JPG)

Now instead of ./run_magic, we use ./gds_magic to run magic with the appropriate tech file to view the seal ring. We can then see the correct seal ring with the read command.

</details>

<details><summary> Lab For Latchup and Antenna Rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e40.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e41.JPG)

Here we have a layout that violates some of the basic rules and latch up rules.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e42.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e43.JPG)

For fixing this, we need to add a tap cell to the design. Align the tap cell accordingly until the drc violations are no longer shown.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e44.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e45.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e46.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e47.JPG)

In this example, we have a long routing happening in the deisgn which would lead to an antenna violation.

Running electrical check is done with the necessary knowledge of the circuit, meaning extraction needs to be performed. The above commands run the antenna check and reason for violation.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e48.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e49.JPG)

The ratio of area of metal to the area of metal to gate is more than twice the allowed value of 400. We can fix this by tying down the route to a piece of diffusion to act as a diode. Since this occurs on metal 2, we need a standard cell diffusion diode anywhere at metal 2, which is already present in the design, we simply need to wire the input where violation starts to the diode.

If we run extraction and antenna check again, we will not see any issues.
 
</details>

<details><summary> Lab For Density Rules </summary>

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e50.JPG)

Here we have a large design containing of metal 1 and 2 layers. We run the above commands to check the metal coverage.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e51.JPG)

Foundries don’t check the average density across whole layout, but do complicated calculations over fixed windows to find densities. We can use a script in magic to perform the calculations based on a script from the sky130 pdk, and with the gds file written.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e52.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e53.JPG)

Running the file above shows us the errors for the file.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e54.JPG)

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e55.JPG)

We then use a fill generator script along with the magic file for the design to create a fill pattern.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e56.JPG)

If we read the gds file generated, we see the fill pattern for the entire layout.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e57.JPG)

We can see a specific layer using the commands above. 

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e60.JPG)

We need to then merge the fill pattern gds to the original file. The positioning of the two needs to be aligned exactly using the commands above.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e58.JPG)

We can view just the metal 2 layer, meaning the fill pattern was aligned perfectly after the merge.

![](https://github.com/YishenKuma/sd_training/blob/main/day28/e59.JPG)

Checking the density coverage with the same commands, we see that the metal 1 density is now within allowable limits. Metal 3 has also been filled now, and within the density limits. 

</details>

</details>

</details>

</details>






