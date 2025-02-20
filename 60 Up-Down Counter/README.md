Copyright 11/17/24, Abby Holdcraft and Camden Smith  
This project uses D flip flops to create up/down base-6 and base-10 counters.

## To Run
Open file in Logisim.  
In the main circuit, enable ticks. To change counting direction, toggle the input labeled "Up/Down Toggle".

## Implementation
### Figures
The following references images found in Tables.pdf
When x=0: the output will be the input plus one, except for when the input is 9. In that case, the output is 0.
When x=1: the output will be the input minus one, except for when the input is 0. In that case, the output is 9.
There is another output called is_9_or_0 that is always 1 except for when x=0 and output=9, OR when x=1 and output=0.
### 6_counter
When x=0: the output will be the input plus one, except for when the input is 5. In that case, the output is 0.
When x=1: the output will be the input minus one, except for when the input is 0. In that case, the output is 5.
### main
These counters were implemented so that the base-10 counter is connected to a clock, and the base-6 counter is connected to the is_9_or_0 output of the base-10 counter. These counters were connected to two seven-segment displays so that when x=0 it counts up from 00 to 59, and when x=1 it counts down from 59 to 00, without the need for a reset button.