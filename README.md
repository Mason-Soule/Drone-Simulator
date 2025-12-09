Drone Simulator – MAVLink SITL Controller

A Python-based drone controller that communicates with a Software-In-The-Loop (SITL) drone using pymavlink. It provides an interactive terminal menu for takeoff, landing, waypoint missions, payload-drop simulation, and return-to-launch behavior.
This project is compatible with ArduPilot SITL, and Mission Planner for monitoring flight data and viewing telemetry.

✨ Features
🛫 Manual Flight Commands

Armed takeoff to a user-selected altitude
Autonomous landing
Return to Launch (RTL)
Guided mode takeoff and altitude tracking

📍 Waypoint & Mission Handling

Full MAVLink mission protocol
Sends waypoint missions using MISSION_ITEM_INT
Automatically starts missions in AUTO mode
Works alongside Mission Planner so you can:
Watch real-time telemetry
View waypoints on the map
Confirm mission uploads
Monitor altitude, GPS, and battery

📦 Payload Drop Simulation

Random target generation
GPS-based navigation to the drop zone
“Drop” event triggered when within 5m of target
Automatic RTL after payload deployment

🔄 Flight Mode Switching

Supports common ArduPilot modes:
GUIDED
AUTO
LAND
RTL
STABILIZE

🧰 Technologies Used

Python Libraries
pymavlink — MAVLink communication
time, math, random, threading

Simulation Tools

ArduPilot SITL
Mission Planner (optional but recommended):
view live flight,
map position,
verify commands,
visualize altitude, GPS lock, and heartbeat
