# FPGA_I2C_BUS_Controller

## Mealy Finite-state machine
* A 13-state finite state machine (FSM) models a sequential logic circuit that controls the output enable of the I/O pins of the FPGA, which are connected to the master and slave clock buses. This FSM is also responsible for detecting whether the slave is busy and holding the clock bus low, which causes clock stretching.
* The state transitions are related to the rising and falling edges of the master and slave clocks, the direction of the write operation (i.e., the device controlling the data (SDA) bus), and the signals that indicate whether the slave is ready and no longer holding the clock bus low.<br><br>
State Diagram:
<img src="Images/FSM_1_Tek.jpg" alt="Alt text" width="1000"><br>
## Moore Finite-state machine
<img src="Images/FSM_2_Tek.jpg" alt="Alt text" width="1000"><br>
