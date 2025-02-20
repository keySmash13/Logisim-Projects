Copyright 10/3/24, Abby Holdcraft and Camden Smith  
This project contains counting displays for decimal and hexadecimal bases.

# To Run
Open file in Logisim.  
Select your desired main circuit, enable ticks (by hitting ctrl + k or select Simulate > Ticks Enabled), enable changing values in the circuit (by hitting ctrl + 1 or selecting the red pointer finger icon in the top left), and click on the object labeled CLOCK.  
To edit speed, select Simulate > Tick Frequency > your preferred speed.  
To terminate, clock on CLOCK again or deselect Ticks Enabled.  

# Decimal Counter
The decimal counter can be found under main_decimal. It uses a clock input and runs it through dec_counter and dec_7seg_driver to display numbers once the simulation is run. 
# Hexadecimal Counter
The hexadecimal counter can be found under main_hexadecimal. It uses a clock input and runs it through hex_counter and hex_7seg_driver to display hexadecimal code once the simulation is run.


# K-Maps
K-Maps used to find minimum SOPs for dec_7seg_driver:  
https://docs.google.com/presentation/d/1U9YnafSg7sMVaW3M8xvBBDHKYSjGGV19Gnm2Lqq1gQg/edit?usp=sharing  
  
K-Maps used to find minimum SOPs for hex_7seg_driver:  
https://docs.google.com/presentation/d/15wl4C3859YrbKpciTF8IMWJjX3F_vvWIAXCNz9v56MI/edit?usp=sharing