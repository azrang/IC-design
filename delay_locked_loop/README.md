DLL consists of three subblocks in total (PFD, Charge pump, and VCDL). Below is the Verilog-A model I created. 
Each block consists of verilog code to test the functionality. 

![Picture7](https://github.com/user-attachments/assets/054a1b71-3a9f-48e0-a069-6363b21aa73a)

I had to verify the functionality of entire DLL under two initial conditions (1. Vctrl = 0V 2.
Vctrl = 1V) 
  - Is ‘UP’ correct? 
  - Is ‘DN’ correct? 
  - Is ‘Vctrl’ changed correctly? 
  - Is output of VCDL (delayed clock) delayed or pulled in correctly? 
