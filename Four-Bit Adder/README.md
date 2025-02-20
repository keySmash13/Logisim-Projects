Copyright 11/5/24, Abby Holdcraft and Camden Smith  
This project demonstrates the use of four-bit adders and multiplexers to four-bit numbers in Logisim.

## To Run
Open file in Logisim.
### Normal Inputs
In the main circuit, configure the input pins as two numbers in binary. It should display both numbers and their solution.
### Multiplexers
The multiplexer is used to select one of the four-bit binary numbers to be added in the display. In the main circuit, configure the number you wish to add and use the multiplexer to select that number. When the multiplexer is set to 0, it will select Number 0, and so on.

## Implementation
### Figures
The following references images found in Tables.pdf
### Adder
The 4-bit adder was implemented though the iterative process of combining eight multiplexers. One multiplexer is used to add binary, using two bits to select an output. The other determines if there is a carried input. Then the output of the carrying multiplexer serves as the input into the next adding multiplexer, effectively allowing us to carry over outputs for situations such as 01+01=10.  
Figure 1 shows the truth table used for this section.
### Tens and Ones
The output of the adder must be converted from binary to BCD, which was done as follows:
The k-map in Figure 2 was used to determine the sum's 10s digit.  
The truth table in Figure 3 was used to determine the sum's 1s digit.
### Multiplexer
Used to select from multiple inputs.
### dec_7seg_driver
Converts BCD to inputs for the seven segment display.