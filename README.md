Download Link: https://assignmentchef.com/product/solved-cda4203l-lab3-bcd-counter-and-fpga-download
<br>
<strong>Objective:  </strong>To learn and practice advanced sequential hardware design in Verilog and synthesizable Verilog based circuit implementation on FPGA board.




<table>

 <tbody>

  <tr>

   <td width="91">Port</td>

   <td width="77">Width</td>

   <td width="38">I/O</td>

   <td width="130">Function</td>

  </tr>

  <tr>

   <td width="91">max_count</td>

   <td width="77">7</td>

   <td width="38">I</td>

   <td width="130">Set the maximum counter value</td>

  </tr>

  <tr>

   <td width="91">run</td>

   <td width="77">1</td>

   <td width="38">I</td>

   <td width="130">Set run mode;0 = set, 1=run</td>

  </tr>

  <tr>

   <td width="91">digit_2</td>

   <td width="77">4</td>

   <td width="38">O</td>

   <td width="130">Ten digit BCD output</td>

  </tr>

  <tr>

   <td width="91">digit_1</td>

   <td width="77">4</td>

   <td width="38">O</td>

   <td width="130">Ones Digit BCD output</td>

  </tr>

 </tbody>

</table>




Figure 1: Counter Top-Level Block Diagram

Table 2

<table>

 <tbody>

  <tr>

   <td width="101">Port</td>

   <td width="59">Width</td>

   <td width="38">I/O</td>

   <td width="116">Component</td>

   <td width="222">Mapping</td>

  </tr>

  <tr>

   <td width="101">Run</td>

   <td width="59">1</td>

   <td width="38">I</td>

   <td width="116">Dip Switches</td>

   <td width="222">SW7</td>

  </tr>

  <tr>

   <td width="101">Max_count</td>

   <td width="59">7</td>

   <td width="38">I</td>

   <td width="116">Dip Switches</td>

   <td width="222">SW6 (MSB) – SW0 (LSB)</td>

  </tr>

  <tr>

   <td width="101">Clk</td>

   <td width="59">1</td>

   <td width="38">I</td>

   <td width="116">Dip Switches</td>

   <td width="222">USER_CLK</td>

  </tr>

  <tr>

   <td width="101">Digit_1</td>

   <td width="59">4</td>

   <td width="38">O</td>

   <td width="116">GPIO LEDS</td>

   <td width="222">LED3 (MSB) – LED0 (LSB)</td>

  </tr>

  <tr>

   <td width="101">Digit_2</td>

   <td width="59">4</td>

   <td width="38">O</td>

   <td width="116">GPIO LEDS</td>

   <td width="222">LED7 (MSB) – LED4 (LSB)</td>

  </tr>

 </tbody>

</table>




<strong>Description: </strong>

Design a programmable counter that outputs BCD and has a range of 0-99. The counter must count from zero to a user-input value. The valid input range is 0-99; if a higher number is input, the counter must not output beyond 99 (decimal). The output from your design should be in binary-coded decimal. You will need to design a binary counter that counts at least to 99<sub>dec</sub>, and a module which converts the binary output to two-digit BCD. A single-bit input, called run, determines the operation of the counter. When run is ‘0’, the counter is set to zero and does not count. The user can set the maximum value here, using an input called max_count. When run is set to ‘1’, the counter starts counting from zero, and stops when it reaches the maximum. Any changes to max_count is ignored when run is set to ‘1’. Your design will have two 4-bit outputs; digit 1 and digit 2. Each is used to output one BCD digit. Digit 2 is the tens digit, digit 1 is the ones digit.

<ol>

 <li>Create a Verilog design (See Figure 1) which will provide the required functionality.</li>

 <li> Exhaustively test the design to ensure that it works under all conditions.</li>

 <li>Use <u>100 MHz</u> to synthesize and map the design on ANVYL board using table 2.</li>

</ol>

<strong>Deliverables: </strong>(1) A concise PDF report that includes your Verilog code and simulation results; (2) A zipped file of your design files (Verilog Models and test benches.) Include a README file. Organize your files in folders named Problem1, Problem2.

<strong>Report Organization (A template is provided on Canvas):</strong>

<ul>

 <li>Cover sheet</li>

 <li>Problem 1 and 2: Verilog Code, Test Bench, and Simulation Results (Waveforms)</li>

 <li>Problem 3: Pin Mapping file</li>

 <li>Feedback: Hours spent, Exercise difficulty (Easy, Medium, Hard)</li>

</ul>

<strong> </strong>