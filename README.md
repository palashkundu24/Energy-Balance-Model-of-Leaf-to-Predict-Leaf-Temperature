## Description: 
This repository contains files and code for the energy balance model of leaf to predict the canopy temperature. This repository is created for the semester project of SOIL 6583: Soil Physics with Python course.


## Leaf Energy Balance: 
The energy balance model allows an estimation of energy loss by transpiration, which is dependent on the gradient of water vapor from the leaf to the atmosphere and the total conductance to water vapor ( the ease with which water vapor diffuses through stomatal pores and the boundary layer).

## First we assume that the leaf is not in contact with the ground. In that case, soil conduction will be zero. Then the surface energy balance for the leaf is expressed as follows:
 Rnet = H+ LE + S 
where, Rnet = Net radiation absorbed by the leaf, H = Sensible heat flux, LE = Latent heat flux and S= Heat storage 


## Constant Assumption for the Model:

# Constants
1. ML = 2  # Leaf mass per unit projected surface area (g/m^2)
2. Cl = 4197  # Leaf specific heat capacity (J/kg*K)
3. ALBEDO = 0.2
4. STEFB = 5.67e-8  # Stefan-Boltzmann constant (W/m^2*K^4)
5. EMISS = 0.75  # Long-wave emissivity of atmosphere
6. BOWEN = 0.5  # Bowen Ratio





