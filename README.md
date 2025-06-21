# moscow128_drl_replacement
Why?  
On my board the 5 pins responsible for the DRL gate were cut on my 2DS627 without a chance to fix it. Also I don't have access to 537RU10 SRAMs or KT3102B transistors. Also happened to have 20 74ALS27 around without a project for them yet.  

What?  
Should be fairly obvious. Solder in 74LS27, place turned 24pin socket in holes, solder in place. Optionally solder in 10K-20K (I used 15K) resistors when using 6116 SRAMs and remove them from the Moscow-128 board (or leave them out on the daughterboard and replace them).  
This shouldn't add more height than 1-2 sockets, depending on how it's soldered. Holes are big enough to fit it onto the underside of a turned socket, might require slightly thinner PCBs than usual - not a problem with most manufacturer's tho from experience.  
You might also want to add 1N4148 diodes facing the data lines for the keyboard (D0-D4) on D44.  

Successfully tested on perfboard with a HM6116LP-2  

Big thank you to Serg6845 from zx-pk.ru for helping me out.  
