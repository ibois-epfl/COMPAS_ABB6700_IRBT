# Instructions
https://ethz.zoom.us/rec/play/6ApGjsRP12yb3BqKNvhnIPZzc8klT_8e712Jtmwb9DWv4jj8IUtMCBhvxfYH0wAlcJqjZ3SCpTbUgASd.V6t5Py49xfJr0Q4r?startTime=1663676217000

## abb_experimental
- [x] Clone repo "abb_experimental" https://github.com/ros-industrial/abb_experimental
- [x] Copy similar model and change names to 6700_175_305 (two urdf xacro files )
- [x] Create .stl files for 3 links -> C:\IBOIS57\_Code\Software\abb_experimental\abb_irb6700_support\meshes\irb6700_175_305\visual
- [x] Create .stl files for low poly geometry -> C:\IBOIS57\_Code\Software\abb_experimental\abb_irb6700_support\meshes\irb6700_175_305\collision
- [x] Coordinates of each axis file -> C:\IBOIS57\_Code\Software\abb_experimental\abb_irb6700_support\urdf\irb6700_175_305.xacro
- [x] finish up the moveit config: https://gramaziokohler.github.io/compas_fab/latest/examples/03_backends_ros/08_ros_create_moveit_package_from_custom_urdf.html
![image](https://user-images.githubusercontent.com/18013985/192538639-b5f09ea0-ba8c-4dfe-8b3c-94aa807c12ab.png)
- [x] check if the package is running in compas_fab, mainly you need to check if meshes are correctly rotating:
![image](https://user-images.githubusercontent.com/18013985/192539156-75078ff9-8c96-4450-b0e9-093a2f1fe3b2.png)

- [ ] cross check results of the IK solver against the values of RobotStudio (this could be done programmatically, using compas_fab to calculate IK solutions from frames and then using compas_rrc to control a RobotStudio virtual controller and verify that both are a match).
- [ ] submit a pull request to ROS-Industrial to add the new model to the upstream abb_experimental repository.


## compas custom repository for IBOIS robot control
- [x] create repository "COMPAS_ABB6700_IRBT" -> https://github.com/ibois-epfl/COMPAS_ABB6700_IRBT/blob/main/docker-compose.yml
- [x] create file docker-compose.yml
- [x] install XLaunch, by download from 
- [x] compose docker, now the move it should open: https://sourceforge.net/projects/vcxsrv/
![image](https://user-images.githubusercontent.com/18013985/191273672-6817796f-10f3-4169-b961-9572e6b9f511.png)
- [ ] create a new support package for the linear axis + the robot mounted on it

