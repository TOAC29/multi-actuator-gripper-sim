# Multi-Actuator Gripper Simulation

Simulation workflows for the multi-actuator soft gripper drive.

## Overview

This README contains the CAD geometry, material characterization data, and simulation file location. Consult the documentation to see which files produce which simulations.

## Drive Structure
```
├── Single Below CAD + Photos 
    ├── Single Linear Actuator Photos
    ├── Single Linear Actuator 3D Files
        ├── Single Linear Actuator SLDRT Files
            ├── TC_FEA_V5_Single Below.sldrt (0mm cap and 1mm cap on both ends of the bellow)
            ├── TC_FEA_V6_Single Below.sldrt (1mm cap on both ends of the bellow)
            ├── TC_FEA_V7_Single Below.sldrt (most updated:10mm base with a 1mm cap on hollow single bellow)
        ├── Single Linear Actuator STL 
            ├── Single_LinearACT5.STL (correlates to TC_FEA_V7_Single Below.sldrt; used to print pressure testing on               |                           the FRESH printer) 
            ├── Single_LinearACT4.STL (correlates to TC_FEA_V6_Single Below.sldrt) 
            ├── Single_LinearACT3.STL
            ├── Single_LinearACT2.STL
            ├── Single_LinearACT.STL
├── Simplified Multi-Actuator FEA
    ├── Simplified Multi-Actuator Photos 
    ├── Simplified Multi Actuator CAD + Simulation Files
        ├── Simplified Multi-Actuator Simulation Files
            ├── Mechanical_simulation_V2.wbpj (FEA with simplified gripper and simplified end pieces)
            ├── Mechanical_simulation_V1.wbpj (FEA with simplified gripper no simplified end pieces)
            ├── MultiActuator_FEA_4.dscodat (Pressure testing simulation inlet/oulet in discovery)
            ├── MultiActator_FEA_3.dscodat
            ├── MultiActator_FEA_2.dscodat 
            ├── MultiActator_FEA_1.dscodat 
        ├── Simplified Multi-Actuator CAD Files
            ├── TC_FEA_V4_truss_w_needle_block_and_gripper.SLDPRT (Most up-to-date CAD produces Multi-Actuator_V2.wbpj)
            ├── TC_FEA_V3_truss_w_needle_block_and_gripper.SLDPRT (No Modified end piece gripper)
            ├── TC_FEA_V2_truss_w_needle_block_and_gripper.SLDPRT  
            ├── TC_FEA_truss_w_needle_block_and_gripper.SLDPRT
        ├── Ansys Hydrogel Characteristics
            ├── Hydrogel Library.xml (Storage file for kPa range)
            ├── 150-225kPa_Range.xml (Material characteristics with 150- 225 kPa range)
├── Actuator V3 
    ├── Actuator_V3 CAD
        ├── Actuator_V3.step (original step conversion from STL, converted through Fusion)
        ├── Actuator_V3_1.step (Modified Actuator with hole cut in base to allow fluid simulation)
        ├── Actuator_V3.STL (Can not open w/ Solidworks; use Fusion STL to STEP conversion process)
    ├── Actuator_V3 Simulation
        ├── V3_Simulation.wpbj
        ├── V3_3.wpbj (Most up-to-date  version of the 3d conversion to induce bending on the gripper)
        
```
