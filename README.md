# Simulation of LaMB <br> [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

Simulation of LaMB in Gazebo environment.

#### For Real Robot Instruction [visit here]:https://github.com/G1-k/LaMB.git

## Instructions

### Give a star to this repo at the top.

### Launch Gazebo world
`roslaunch lamb_sim room.launch`

### Mapping
`roslaunch lamb_sim gmapping.launch`

Visualization
```
cd /workspace/src/lamb_sim/rviz/
rviz -d mapping.rviz
```
Save Map - `rosrun map_server map_saver -f /workspace/src/lamb_sim/maps/map_name`

### Navigation
```
roslaunch lamb_sim amcl.launch map:='map_name'
roslaunch lamb_sim move_base.launch 
```
### Visualization
```
cd /workspace/src/lamb_sim/rviz/
rviz -d navigate.rviz
```

### License

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
This work/project is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License][cc-by-nc-sa]. Please read the license before replicating the project.<br>
[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

