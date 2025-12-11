As someone who is not a subject matter expert in fusion power conversion, 
I’ve structured the model to be as parameterized as possible with placeholder values wherever needed.  The script takes user-defined inputs such as output power, 
discount rate, project lifespan, etc. to generate an apples-to-apples LCOE comparison.  A pie chart breaks out the key drivers (both positive and negative) behind 
the LCOE change across power conversion types.  

The CAPEX appears to be lower for Direct EM Capture (DEC) because of its smaller footprint (no turbine hall, smaller reactor) and simpler architecture (avoided turbines, 
molten salt storage, BoP infrastructure, and blanket costs).  As for the OPEX, a pulsed DEC reactor generally consumes more auxiliary power because of its lower Q value 
(source:  https://www.helionenergy.com/articles/how-to-make-fusion-electricity-without-ignition/). However, a Thermal-to-Electric (TtoE) reactor will likely have higher 
maintenance costs due to the structural degradation and radioactive waste management that comes with neutronic fusion (source: https://arxiv.org/pdf/2405.01514).  As for 
energy generation, this script fixes the power output across both technologies, but the total generation for DEC will likely be less due to the pulsed nature of aneutronic fusion. 

As a sidenote, I have also embedded the capability for degradation comparisons, though it is currently set to zero for simplicity.  I’ve also included a placeholder value for 
regulatory markup on CAPEX, acknowledging that regulatory costs could differ between conversion types, especially given that DEC produces less radioactive waste than TtoE. 

Please feel free to query the script in the github repo linked above.  You will find that DEC is generally lower cost than TtoE, but this is highly sensitive to certain inputs– 
particularly the capacity factor (%), specific CAPEX (USD/kW), and discount rate (%).
