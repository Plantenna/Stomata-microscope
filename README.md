# Stomata-microscope
Non-invasive microscopic imaging of individual stomatal kinetics in the growth environment 


Stomata regulate the gas exchange with the environment, balancing between water loss and CO2 uptake. Gas-exchange dynamics are influenced by stomatal morphology, size and density that are commonly investigated using imprint and SEM, methods that are destructive and elaborate. Moreover, these microscopic properties are statically sampled and related to the dynamic ensemble behavior: gas exchange of an entire plant or part of a leaf. Little is known on how morphology, size and density of stomata influence the kinetic behavior of individual stomata. The compact microscope system described here measures individual stomatal aperture kinetics of tens of stomata with sub-minute time resolution in vivo in the growth environment with minimal impact to the leaf’s surrounding . Sub-micron apertures can be resolved, capturing the dynamics accurately even at low light intensities. Simultaneous chlorophyll fluorescence, ambient temperature, humidity and light intensity measurements enable the investigation of environmental parameters on the dynamics of individual stomata. The characteristics of our microscope and data analyses are described in this open science project.

Design principle

The microscope is designed to image stomata non-invasively in the growth environment, therefore the following design requirements had to be met:
                  
                  low light intensity for imaging light (to least affect the stomatal behaviour), 
                  
                  high resolution (to resolve minimal apertures), 
                  
                  long working distance (to keep the leaf in its natural surrounding as much as possible), 
                  
                  A clamp that keeps the leaf in position but doesnt affect its physiology
                  
                  control over stimulus light to affect the stomatal behavior
                  
                  Autofocus, to follow the movement of the leaf surface over time on the z-axis when the leaf turgor changes,
                  
                  A speed of imaging that could resolve the surface of the leaf within a minute or less
                  
                 
To meet this requirements we used the following approach:

Imaging light was either green (530 nm) or near infrared (850 nm), the latter with the least impact on the stomatal physiology but with lower resolving power. A filter was used to selectively pass a selected wavelength range to the camera. This choice was made to minimize chromatic abberations and to maximize the sensitivity of the cameras that we employed. Additionally both selected wavelengths are reflected/transmitted well by the leaf surface and thereby enable imaging in bright or darkfield mode.

The microscope objectives used were all from Mitutoyo, ranging from 20x to 50x with numerical apertures (NA) from 0.42 to 0.75 and with working distances (WD) of 5.2 to 20.5 mm. For near infrared (NIR) imaging we used a 50x NIR objective, 0.42 NA, WD 17 mm. 

The imaging light came from an effiring light (https://www.effilux.com/en/products/ring/effi-ring) green or NIR with the focus and the diffuseness of the light optimized for each leaf sample. In a variation, the green light from the PSI LEDS (http://led-growing-lights.com/products/led-lights-sl-3500/) could also be used for imaging. Light intensity used was optimized for each leaf sample. Imaging could be done in brightfield or darkfield mode that was optimized for each leaf sample.

Stimulus light was provided by the PSI LEDs SL3500 (http://led-growing-lights.com/products/led-lights-sl-3500/, Blue and Red light) that could be programmed to affect the spectrum as well as the intensity of the stimulus light over time to simulate fluctuations in the growth environment. Stimulus Light was always provided from the top side.

The leaf was clamped in a 3D printed transparent leaf holder. The leaf was clamped between 3D printed transparent rings with variable diameter with magnets embedded. The magnets aligned with magnets in the holder to have always the same alignment. The ring and the holder both have a ring of inert and soft polymer attached, similar to the Licor6800, to make sure that the clamping was soft enough to keep the leaf in a healthy state. Variants to the holder were created that could hold the fiber optics from a minipam (https://www.walz.com/files/downloads/manuals/mini-pam-II/MINIP_1EB.pdf) at the correct angle towards the topside of the leaf for fluorescence measurements. 

An autofocus function, based on contrast values, was employed to fit a gaussian profile to the z-stack of images at each timepoint to find the optimal focus and to adjust the center point for the next image. Different methods for contrast calculation could be used and were optimized based on the leaf sample.

The camera (https://www.flir.eu/products/blackfly-s-usb3/?model=BFS-U3-244S8M-C&vertical=machine+vision&segment=iis) was used in 12bit mode with 2x2 binning to be able to use the lowest possible light intensity for imaging. The exposure time was optimized for each leaf sample. A typical image stack contained 100 images spaced across 100 micrometer that were acquired over a period of 50 seconds. z-axis depth (stack size) and z-axis step size were adjusted to the leaf and the microscope objectives depth of image, such that distance between images along z was always less than the depth of image of the microscope objective.

The hardware list and 3D model (Solidworks) are in folder stomata microscope mechanical

The labview acquisition software is in folder YY

The ImageJ analyses scripts are in folder ZZ











