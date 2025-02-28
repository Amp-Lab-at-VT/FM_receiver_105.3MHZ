## Members
Phillip Bozzay, Electrical Engineering Student (2027)
phillipb23@vt.edu

Brady Falk, Computer Engineering Student (2027)
bradybop14@vt.edu

## Mentor
Eddie Pritchard 
Yousef Chebil
Nicholas Pacheck

## Current Status
IN THE WORKS NOW 

## Project Overview

Analog radio (100MHz) with a digital interface.
Custom design, PCB design education value is custom RF pcb design and research of relevant components

## Educational Value Added

PCB design education value is custom RF pcb design and research of relevant components

## Tasks


## Design Decisions
General Design Layout: https://docs.google.com/drawings/d/1e5mTtKONOJFI6KM5OiUcPPun2-vZfV_UhMkgm8joVLU/edit?pli=1
- The General design is an analog radio with a digital display
- The radio receiver circuit will be designed for signals between 90 MHz and 107 MHz
- The user will be able to tune the channel via variable capacitor
- A switch will configure the audio input circuit to radio input / regular audio input (cable)
- User will be able to adjust the volume and equalize the audio using potentiometers
- The audio circuit will drive a low resistance speaker 
- Spectrogram, and more information  will be visible via SPI display
  
Digital Display: https://docs.google.com/drawings/d/1l0TOMat3e_Cb2plj9UsGKdRVyu4xmmN-r_CkISbyUpM/edit?pli=1
- Display FFT information
- Display FM channel


SPI Display Driver Circuit
https://docs.google.com/drawings/d/1E67qR3yuNH56lItT9SU0MOQwrdpFbPqokMBX5DFpPCU/edit?pli=1
- The 2.8" TFT SPI display requires the the GPIO inputs be logic shifted from 5 volts to 3.3 volts
- This is a simple voltage divider
- Implementing this on a breadboard is quite messy, so the goal is to put this on a PCB chip
- This driver circuit will be general purpose, not specific to this particular use case 

External Memory Circuit
https://docs.google.com/drawings/d/11PcZ85OOiS_0Ki8MvOQhEjBIvRu9X47G4qPSfKRWTIE/edit?pli=1
- The arduino uno only has 2kb of SRAM. 
- the arduino would require a minimum of 10kb of SRAM (rough estimate) in order to compute and display a low resolution FFT
- This circuit outsources the SRAM to an external chip, which will allow for 256kb of SRAM.
- Goal is place these connections on a PCB 


## Design Misc

## Steps for Documenting Your Design Process

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## BOM + Component Cost

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Timeline
Feb 2/28/2025 validation for audio equalizer circuit successfully completed https://docs.google.com/drawings/d/1Yy9J6RnNpgs11lCt3ADg5ZqFTQz8fsf5LOfN7ywQ5KU/edit?pli=1
NEXT: fm receiver, bluetooth amplfier, selection circuit, and graphic equalizer display on single PCB

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Useful Links

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Log

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->
