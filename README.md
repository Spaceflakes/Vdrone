# Velocidrone IMU Telemetry Logger

This repository contains tools to connect to the Velocidrone simulator's WebSocket telemetry stream, log the drone's IMU and positional data, and visualize its flight path.

## What is the "Publish IMU / Telemetry" feature in Velocidrone?

In the Velocidrone simulator, the **Publish IMU / Telemetry** setting (or "Websocket Communication") enables a local WebSocket server that broadcasts live data from the drone while you are flying. 

When this feature is active, Velocidrone streams high-frequency JSON packets containing the physical state of the drone. This includes:
- **IMU Data**: Roll, Pitch, and Yaw rates.
- **Absolute Position**: X, Y, and Z coordinates of the drone within the simulated environment.
- **Attitude (Quaternions)**: The 3D orientation of the drone.
- **Speed**: Velocity along the X, Y, and Z axes.

This feature is incredibly useful for developers and researchers who want to analyze flight performance, visualize race lines, create custom telemetry overlays, or train external machine learning models on drone dynamics.