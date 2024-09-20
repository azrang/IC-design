For a typical front-end RF circuit especially for WiFi/Bluetooth application, my oscillator needs to drive the mixer. 
Assume that the distance between mixer and oscillator is far away so the output of the oscillator decreases as it travels to mixer.
So, we need Op-amp to boost the oscillator output signal.
I designed a differential input and differential output Op-amp structure. I also did layout without LVS nor DRC errors.

![Screenshot 2024-09-20 113321](https://github.com/user-attachments/assets/74a049b9-bcee-417b-9506-a6de25e23739)

We need an Op-amp which differential peak-to-peak output swing is > 0.8V (singleended peak to peak swing is 0.4V). There are 6 factors we evaluate.
  - fu : Unity gain frequency (Frequency when your gain is 0dB). Your oscillator
operating frequency is equal to 2.4GHz, so we need to meet fu at least 5GHz.
  - Phase margin : it is common to have at least greater than 60o phase margin for
the Op-amp.
  - Power consumption : The target power consumption is 4.5mW
  - Gain : It is important to have a large gain for Op-amp. Let’s target to have
35dB at low frequency ( < 3dB frequency )
  - Peak-to-Peak output amplitude : Each output should have at least 0.4V peak to
peak amplitude at Maximum. (Differential peak to peak amplitude is 0.8V)
  - Common-mode feedback techniques.

