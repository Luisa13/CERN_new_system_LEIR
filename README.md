# New BPM Orbit System in LEIR
This is the work presented in the Beam Instrumentation annual workshop in 2018 where I introduced all the software achievements for the LEIR accelerator.
**LEIR** stands by [Low Energy Ion Ring](https://home.cern/science/accelerators/low-energy-ion-ring), and is a particle accelerator at CERN used to accelerate ions from the LINAC 3 to the PS (Proton Synchrotron ) to provide ions for collisions within the LHC.
Here you can find the system installed for LEIR which allows to measure the positions of the bunched beam.


## Context
On the one hand in the ring orbit we needed to cope with an orbit upgrade (for LEIR) due to an obsolence of the current software so the calibration programs needed to be replaced; On the other hand the low intensity ion beams coming from LINAC3 urged an optimization in the injection line efficiency.


## What was done
#### ORBIT
- New digital acquisition system was installed.
- Driver upgrade was needed for trajectory feature.
- Reuse a previously developed class in order to change it completely. The common class for three compact rings makes the maintenance easier.
#### INJECTION LINE
In order to optimize the injection efficiency into LEIR the transfer line between L3 and LEIR has been equipped with nine highly sensitive electrostatic BPMs.
Therefore, the acquisition system shall be improved in order to allow turn by turn acquisition as well as bunch by bunch acquisition
- The low noise charge amplifier mounted directly on the BPM.
- New control [FESA](http://cds.cern.ch/record/2305325?ln=en) class developed
- The new system gained control and the component will enable to comply the requirement of beam position measurement along the pulse. This required an upgrade of the acquisition system.



Global Overview       |     Expert Overview
----------------------|-------------------------
![](https://user-images.githubusercontent.com/3811449/113399298-48c73f80-93a0-11eb-8e98-3cc7f57cea6a.png) | ![](https://user-images.githubusercontent.com/3811449/113399366-672d3b00-93a0-11eb-89ff-20cb4a0d5eaa.png)

The resulting Expert GUI is helping to debug the new system and it's used operationally by [BI](https://sy-dep-bi.web.cern.ch) and [OP](https://be-dep-op-leir.web.cern.ch)



## Results
In the results presented we reported much more precision comparing the average of the orbit. As far as the standard deviation concerns, we could appreciate the performance for the new system show much less noise. The data is more focused, and less spread out. As conclusion, the new orbit system is used operationally by BI and OP for orbit and trajectory and the software is useful for debugging new features for the first turn positions.

![compNEWOLDLEIR1](https://user-images.githubusercontent.com/3811449/113395094-9c825a80-9399-11eb-8ff1-3c4d4bfbc5f3.png)
![compSTD_NEWOLDLEIR1](https://user-images.githubusercontent.com/3811449/113395152-b15eee00-9399-11eb-9080-d2b79f4b3ad0.png)




## Author
Luisa Sanchez Avivar - 2018

All the corresponding code belongs to [BI-SW department](https://sy-dep-bi.web.cern.ch/sw) repositories.
For more detailed information, please see the complete [presentation at INDICO](https://indico.cern.ch/event/776640/contributions/3230043/attachments/1759118/2863064/Software_in_the_new_BPM_sys._LEIR_1.pdf).


