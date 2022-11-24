# Gas-Permeation-Dual-Piston-Lab
 Pressure Transducer detection and logging
 
 ### User Interface
 ![image](https://user-images.githubusercontent.com/97303986/197994887-c41d5ab4-d10b-47a3-8e76-c728a9c8db6d.png)


## Downloading & Running Software

1. Download Folder `Gas Permeation Rig V1` to local machine.

2. Ensure folder contains the sub folder `Data`

3. Run Gas Permeation Rig.exe
![image](https://user-images.githubusercontent.com/97303986/197995047-d7013b76-6df5-4d33-823b-45db3cec29b1.png)


## Data Aquisition

1. To start sampling data, click the `Start Sampling` button. 
    - Sampling Active Indicator will light if operation is successful
2. To start logging data to CSV file, cick `Start Logging`
    - Logging Active indicator will light to show operation is successful.
    - Data will be saved to CSV File, named YYYY_MM_DD_HH_mm_ss_pressure-data.csv inside `Data` folder
3. Clicking any of the Start logging, Start Sampling or the Exit button will close the open CSV file and perform safe shutdown of hardware.

## Exiting

Press `Exit` at any point to close the software. Any open file will be closed and DAQ device will end process.


## Code Structure

_Adding notes here on implementation as a reference_

![image](https://user-images.githubusercontent.com/97303986/203825895-7cfb44e2-e130-44fe-af37-1ffe8e0ef7fe.png)

Here, two timing loops are used to seperatly trigger both sampling and logging of the datapoints. I think this topology can be refractored to work more seamlessly. See Muscle Actuator project for a new attempt at a similar implementation.
