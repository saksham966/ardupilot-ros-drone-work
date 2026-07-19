🚁 ArduPilot SITL with Gazebo Classic

A complete ArduPilot Software-In-The-Loop (SITL) simulation environment using Gazebo Classic 11 for autonomous UAV development, testing, and research. This project integrates ArduPilot, Gazebo Classic, MAVProxy, and MAVLink to simulate an Iris quadcopter in a realistic physics environment.

📌 Features
🚁 ArduPilot SITL (Software-In-The-Loop) Simulation
🌍 Gazebo Classic 11 Integration
📡 MAVLink Communication
🎮 MAVProxy Ground Control
⚙️ Iris Quadcopter Simulation
🛰️ GUIDED Mode Flight Control
🔧 Plugin-based Gazebo Integration
🐧 Ubuntu Compatible
🛠️ Tech Stack
ArduPilot 4.5
Gazebo Classic 11
MAVProxy
MAVLink
CMake
Git
Ubuntu Linux
📂 Project Structure
ardupilot/
│
├── ardupilot_gazebo/
│   ├── build/
│   ├── models/
│   ├── worlds/
│   └── plugins/
│
├── Tools/
├── build/
└── SITL
🚀 Installation

Clone the repositories

git clone https://github.com/ArduPilot/ardupilot.git
git clone https://github.com/ArduPilot/ardupilot_gazebo.git

Build the Gazebo plugin

cd ardupilot_gazebo
mkdir build
cd build
cmake ..
make -j$(nproc)
▶️ Running the Simulation
Terminal 1

Start Gazebo

cd ~/ardupilot_gazebo
gazebo worlds/iris_arducopter_runway.world
Terminal 2

Start ArduPilot SITL

cd ~/ardupilot

Tools/autotest/sim_vehicle.py \
-v ArduCopter \
-f gazebo-iris \
--console \
--map
✈️ Basic Flight Commands
mode GUIDED

arm throttle

takeoff 10

land
📸 Simulation

The simulation consists of:

Iris Quadcopter
Gazebo Physics Engine
MAVProxy Console
Interactive Map
MAVLink Communication
🎯 Learning Outcomes
Built ArduPilot from source
Integrated Gazebo Classic plugin
Configured Iris UAV model
Established MAVLink communication
Learned SITL workflow
Explored autonomous UAV simulation
Debugged simulation and plugin integration
🔮 Future Work
ROS 2 Integration
MAVROS Communication
Offboard Control
Autonomous Waypoint Navigation
Computer Vision Integration
Object Detection using YOLO
SLAM-based Navigation
Multi-UAV Simulation
🤝 Contributing

Contributions are welcome!

Fork the repository
Create a feature branch
git checkout -b feature-name
Commit your changes
git commit -m "Add feature"
Push the branch
git push origin feature-name
Open a Pull Request
📄 License

This project uses the open-source licenses of the underlying software, including ArduPilot and Gazebo. Refer to their respective repositories for license details.

🙋 Author

Saksham Badal

🎓 Integrated M.Tech, Applied Geophysics, IIT (ISM) Dhanbad
🤖 Robotics & Autonomous Systems Enthusiast
🚁 UAV Simulation | ROS 2 | Computer Vision | AI

⭐ If you found this project useful, consider giving it a star!
