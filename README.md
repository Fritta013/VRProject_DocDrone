# VRProject_DocDrone


# Introduction 🚀

This project involves creating a virtual control room using Unreal Engine 4.27 and the AirSim plugin, which provides a detailed simulation environment for smart ambulance drone (UAV) in medical payload transport. The simulation features various types of terrain, urban landscapes, and obstacles that these vehicles must navigate. It allows for the testing and validation of different sensors, including LIDAR, RGB, and thermal cameras.

The simulation supports the development and validation of algorithms for path planning, navigation, and real-time data collection. It enables the integration of new features and applications into the vehicle's hardware and software. Furthermore, the use of AI and machine learning algorithms in the simulation enhances the precision and efficiency of navigation and data analysis, contributing to the overall advancement of medical transport solutions.


## Objectives

1. **Integrate navigation sensors** such as GPS and barometers.
2. **Create a mission generator and logging system** for data recording and analysis.
3. **Ensure platform compatibility** with Windows and Linux.
4. **Analyze mission performance and UAV health** in a control center.
5. **Ensure carrying medicines from the medical center** to the patient in a square path passing by charging stations.

## Tools and Components

### AirSim/PX4 Specifications

- **Safety:** Failsafe, geofencing, return to home (RTH).
- **Control:** Attitude, Position, Velocity.
- **Flight Modes:** Manual, Stabilized, Altitude, Position, Offboard, Mission.
- **Hardware:** Supports various flight controllers, GPS modules, IMUs, barometers.

### Unreal Engine Environment

- **Graphics:** High-fidelity, real-time rendering.
- **Landscapes:** Customizable terrains.
- **Version:** Unreal Engine 4.27.
- **Integration:** Uses Cesium for 3D environments, Google Maps for real-world data, and Landscape Mountain for terrain.


![Flowchart](dronefinal.png)


## Install Epic Game Launcher & Unreal Engine 4.27 🛠️

## Download Package 📦

To download the project files, clone this project and look for "setting.json" file. Copy this file in Airsim folder inside your main project. 

1. **Extract Files**

   - **Drone_VR Folder:** Contains the Unreal Engine environment. Extract it into the `Documents\Unreal Projects` directory.
   - **Drone_shell Folder:** Contains the cpp and Python scripts. Extract it into the AirSim folder you downloaded. Note that there's already a file named "Drone_shell" inside the AirSim package, so you'll need to replace it with the one from the project files. The program is written in python, the name of the python file to run is `DocDronefinal.py` .

2. **Compile Program** 🖥️

   After adding the `Drone_shell` file and extracting it, you can use the Developer Command Prompt VS22 to navigate to the repository where you put the AirSim package. Then, you can call `build.cmd` to compile the program and generate the "Plugin" folder for Unreal Engine.

3. **Copy Files** 📂

   - **Drone_shell File:** Copy the `Drone_shell` file from the AirSim package and paste it into the `Documents\Unreal Projects\VRProject_DocDrone` folder.
   - **Plugin File:** Copy the `Plugin` file from the `AirSim\Unreal` package and paste it into the `Documents\Unreal Projects\VRProject_DocDrone` folder. There may already be a "Plugins" folder inside the "VRProject_DocDrone" directory. Simply replace it with the new one from the AirSim package.

4. **Generate Visual Studio Project Files** 📄

   Right-click on the `Airsimtest2022.uproject` file in the `VRProject_DocDrone` folder and select **Generate Visual Studio project files** to perform the final compilation of the project with the newly added files.

5. **Open the Project** 🔧

   Open the `Airsimtest2022.sln` file and ensure that the configuration solution is set to `Debug Game Editor` and the solution platform is set to `Win64` and start the project. The initial compilation may take some time. If the Unreal environment does not open, try restarting the project.

## AirSim Plugin Setup 🛸

If you're using the AirSim plugin for the first time in Unreal Engine, follow these steps:

1. **Check Plugin Installation** 🔍

   - Go to **Edit/Plugins** and search for "AirSim".

2. **Set Game Mode Override** 🎮

   - Go to **Window/World Settings** and set the GameMode Override to `AirSimGameMode`.

3. **First-Time Setup** 🛫

   - When you first play the game, Unreal will ask you which type of vehicle you want to use with AirSim. Select one and start playing.

4. **Optimize Performance** ⚙️

   - Go to **Edit/Editor Preferences**, search for "CPU", and uncheck the option **Use Less CPU when in Background**. This ensures optimal performance by preventing Unreal Engine from slowing down when the window loses focus.

5. **Update Settings** 📁

   - Stop the game and close the environment. In your Documents folder, find the `AirSim` folder created automatically after the first run. Inside, replace the existing `settings.json` file with the one you downloaded from our Google Drive.

6. **Reopen Project** 🚀

   - Reopen the `Drone_VR.sln` file in your Unreal project folder. The changes in the new `settings.json` file and the existing file will merge automatically.

## Demo Video: 


## Students:

- Ines Haouala
- Benkredda Roumaissa
- Karim Triki
