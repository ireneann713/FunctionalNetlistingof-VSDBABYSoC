# FunctionalNetlistingof-VSDBABYSoC


## FUNCTIONAL SIMULATION

A functional simulation simulates the design description to verify its logical correctness. A circuit represented in the form of logic expressions can be simulated to verify that it will function as expected. The tool that performs this task is called a functional simulator.

![image](https://user-images.githubusercontent.com/55539862/178995072-9dab76bc-da90-49f3-bfed-7e5ff88f76eb.png)


## Simulation of VSDBABY SoC

![image](https://user-images.githubusercontent.com/55539862/183136639-11da7fc6-97f4-4d80-b1d3-1ed202a68ae8.png)

  * **CLK:** This is the `input CLK` signal of the `RVMYTH` core. This signal comes from the PLL, originally.
  * **reset:** This is the `input reset` signal of the `RVMYTH` core. This signal comes from an external source, originally.
  * **OUT:** This is the `output OUT` signal of the `VSDBabySoC` module. This signal comes from the DAC (due to simulation restrictions it behaves like a digital signal which is incorrect), originally.
  * **RV_TO_DAC[9:0]:** This is the 10-bit `output [9:0] OUT` port of the `RVMYTH` core. This port comes from the RVMYTH register #17, originally.
  * **OUT:** This is a `real` datatype wire which can simulate analog values. It is the `output wire real OUT` signal of the `DAC` module. This signal comes from the DAC, originally.
![image](https://user-images.githubusercontent.com/55539862/184079814-4a9ac1a8-c9f5-4873-8732-0017f6032ed7.png)


## ACKNOWLEDGEMENTS

  * Kunal Ghosh, Co-Founder (VLSI SYSTEM DESIGN - VSD)
  
## References
   * https://www.vlsisystemdesign.com/rtl-design-using-verilog-with-sky130-technology/?q=%2Frtl-design-using-verilog-with-sky130-technology%2F&v=a98eef2a3105
   * https://github.com/kunalg123/vsdflow
   * https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop
   * https://github.com/google/skywater-pdk


