# ros2-rover-navigation

## Following Steps
1. `mkdir ros2-rover-navigation` `cd ros2-rover-navigation/` `mkdir src` `cd src/`
2. `ros2 pkg create --build-type ament_python --node-name rover_navigation_node rover_navigation_pkg`
3. `cd rover_navigation_pkg/` `code .`
4. create a folder named `urdf`
5. inside urdf folder, create a file name `my_rover.urdf`
6. write my urdf code
7. go to terminal, `cd urdf/`
8. `ros2 launch urdf_tutorial display.launch.py model:=/home/mahfuz/ros2-rover-navigation/src/rover_navigation_pkg/urdf/my_rover.urdf`
9. open the vs code, create folders named `launch` and `rviz`
10. `ros2 launch urdf_tutorial display.launch.py model:=/home/mahfuz/ros2-rover-navigation/src/rover_navigation_pkg/urdf/my_rover.urdf`
11. save config as in rviz folder named `config.rviz`
12. creates `display.launch.py` and `gazebo.launch.py` files in launch folder
13. make `display.launch.py` and `gazebo.launch.py` files are executable
14. modify the `setup.py` code
15. `cd` `cd ros2-rover-navigation/` `colcon build --symlink-install`
16. `source install/local_setup.bash`
17. modify `display.launch.py` code
18. 
