# VRProject_DocDrone



## Project Overview

This project aims to create a simulated control room using Unreal Engine 4.27, integrating AirSim to simulate smart ambulances (UGVs) and drones (UAVs) for medical payload transport. The system features real-time path planning using 2D map data from Cesium or Google Maps and includes sensor integration for navigation and monitoring. The platform supports both Windows and Linux environments using Unreal Engine, AirSim, PX4, D-Flight API, and Python scripting.

## Objectives

1. **Develop real-time path planning for UGVs** using 2D maps from Cesium or Google Maps.
2. **Integrate navigation sensors** such as GPS and barometers.
3. **Create a mission generator and logging system** for data recording and analysis.
4. **Ensure platform compatibility** with Windows and Linux.
5. **Analyze mission performance and UAV health** in a control center.

## Tools and Components

### AirSim Vehicles

- **Multirotors:** For aerial tasks like photography and inspection.
- **Fixed-Wing Aircraft:** For aviation applications.

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


![Flowchart](path/to/dronefinal.png)

## Getting Started

### DroneShell API Control

1. Start the Unreal Engine project and press Play.
2. Run DroneShell.exe in the AirSim folder.
3. Use commands like RequestControl, Arm, TakeOff, Land.
4. Type `help` for additional commands.

### PX4 SITL API Control

- Runs on Linux, communicates with PX4 using MAVLink API.
- Uses UDP (Ports 14550 or 18570) and TCP (Port 4560).
- Requires LocalHostIP and ControlIP configuration.

### Python API Control

- Controls position, altitude, weather, and more using Python.
- Example trajectory: Hospital > Charging Station 1 > Patient > Charging Station 2 > Hospital.
- Coordinates: (125, 0), (125, -130), (0, -130), (0, 0).

## Enhancements and Future Work
- Upgrade to Unreal Engine 5.3/5.4 for advanced simulation.
- Incorporate machine learning for autonomous navigation and efficiency.
- Implement real-time analytics for mission performance using drone RGBD cameras.

## Students:

- Ines Haouala
- Benkredda Roumaissa
- Karim Triki
