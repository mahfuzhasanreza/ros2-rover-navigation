# ros2-rover-navigation

## Following Steps
1. `mkdir ros2-rover-navigation` `cd ros2-rover-navigation/` `mkdir src` `cd src/`
2. `ros2 pkg create --build-type ament_cmake --node-name rover_navigation_node rover_navigation_pkg`
3. `cd rover_navigation_pkg/` `code .`
4. create a folder named `urdf`
5. inside urdf folder, create a file name `my_rover.urdf`
6. write my urdf code
7. go to terminal, `cd urdf/`
8. open the vs code, create folders named `launch` and `rviz`
9. `ros2 launch urdf_tutorial display.launch.py model:=/home/mahfuz/ros2-rover-navigation/src/rover_navigation_pkg/urdf/my_rover.urdf`
10. save config as in rviz folder named `config.rviz`
11. creates `display.launch.py` and `gazebo.launch.py` files in launch folder
12. make `display.launch.py` and `gazebo.launch.py` files are executable
13. modify the `setup.py` code:
      ```
      # Install launch files.
      install(DIRECTORY
        launch
        urdf
        rviz
        DESTINATION share/${PROJECT_NAME}/
      )
      ```
14. `cd` `cd ros2-rover-navigation/` `colcon build --symlink-install`
15. `source install/local_setup.bash`
16. modify `display.launch.py` and `gazebo.launch.py` codes
17. `ros2 launch rover_navigation_pkg gazebo.launch.py`
18. `ros2 run teleop_twist_keyboard teleop_twist_keyboard`


## Important
1. `ros2 launch urdf_tutorial display.launch.py model:=/home/mahfuz/ros2-rover-navigation/src/rover_navigation_pkg/urdf/my_rover.urdf`
2. `ros2 launch rover_navigation_pkg display.launch.py`
3. `ros2 launch rover_navigation_pkg gazebo.launch.py`
