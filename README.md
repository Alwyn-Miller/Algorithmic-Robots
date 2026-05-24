# Algorithmic-Robots
This Repo contains the final working components created by Alwyn and Hamish for the UC algorithmic robotics class.

# To Clone This Repo
```
git clone https://github.com/Alwyn-Miller/Algorithmic-Robots.git
```


# To Open Simulated Environment
```
cd algorithmic-robots-world
docker compose -f compose-simulation.yaml pull
xhost +local:root
docker compose -f compose-simulation.yaml up
```


# To Open Physical Robot Environment 
```
cd algorithmic-robots-world
docker compose -f compose-physical.yaml pull
xhost +local:root
docker compose -f compose-physical.yaml up
```
Once the environment is up use a browser navigate to http://127.0.0.1:8080.
This browser-based VS code interface already has ROS 2 and the TurtleBot dependencies pre configured.

# To Build And Run
```
cd /workspace/succulence_ws
colcon build --packages-select succulence_rover_ros --symlink-install
source install/setup.bash
```
In a second terminal run the code below followed by the desired file ie: succulence_rover_ros mission.launch.py
```
ros2 launch 
```
Open Rviz 
```
Rviz2
```



# Work Breakdown
## work was accomplished together during tutorials, but depending on the week and system issues, work was primarily done on one of our two devices:
| Component | Contributor |
| ------------ | ------------- |
| Motion Model | Alwyn  |
| Occupancy Grid | Hamish |
| Scan Matcher | Alwyn  |
|Pose Graph SLAM | Hamish  |
| A* and Navigator | Both  |

