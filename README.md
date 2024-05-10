## Description: 
This repository contains files and code for the energy balance model of leaf to predict the canopy temperature. This repository is created for the semester project of SOIL 6583: Soil Physics with Python course.


## Leaf Energy Balance: 
The energy balance model allows an estimation of energy loss by transpiration, which is dependent on the gradient of water vapor from the leaf to the atmosphere and the total conductance to water vapor ( the ease with which water vapor diffuses through stomatal pores and the boundary layer).

## First we assume that the leaf is not in contact with the ground. 
In that case, soil conduction will be zero. Then the surface energy balance for the leaf is expressed as follows:
 Rnet = H+ LE + S 
where, Rnet = Net radiation absorbed by the leaf, H = Sensible heat flux, LE = Latent heat flux and S= Heat storage 

## Constants
1. ML = 2  # Leaf mass per unit projected surface area (g/m^2)
2. Cl = 4197  # Leaf specific heat capacity (J/kg*K)
3. ALBEDO = 0.2
4. STEFB = 5.67e-8  # Stefan-Boltzmann constant (W/m^2*K^4)
5. EMISS = 0.75  # Long-wave emissivity of atmosphere
6. BOWEN = 0.5  # Bowen Ratio

## Model Overview:
1. Input Data: The model uses environmental data such as solar radiation (SRAD) and air temperature (TAIR) to predict the leaf temperature (TLEAF).
2. Net Radiation Calculation: The calculate_net_radiation function computes the net radiation received by the leaf, considering incoming shortwave radiation, outgoing longwave radiation, and atmospheric emissivity.
3. Sensible Heat Flux Calculation: The calculate_sensible_heat_flux function estimates the sensible heat flux between the leaf and the surrounding air.
4. Latent Heat Flux Calculation: The calculate_latent_heat_flux function computes the latent heat flux, representing the energy exchange due to evapotranspiration.
5. Temperature Change Calculation: The calculate_temperature_change function calculates the rate of change of leaf temperature based on the net radiation, sensible heat flux, and latent heat flux.
6. Prediction Loop: The model iterates over each time step in the dataset, updating the leaf temperature based on the calculated temperature change.
7. Comparison: Finally, the predicted leaf temperatures are compared with the actual leaf temperatures from the dataset.



