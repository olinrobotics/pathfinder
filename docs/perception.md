# Neato Perception Stack

## Neato Perception (Simulator)
roslaunch neato_simulator neato_playground.launch

rosrun map_server map_server `rospack find neato_2dnav`/maps/playground_smaller.yaml

roslaunch neato_2dnav amcl_builtin.launch map_file:=`rospack find neato_2dnav`/maps/playground_smaller.yaml


## Neato Perception (Onboard)
roslaunch neato_node bringup.launch host:=192.168.xxx.xxx

roslaunch neato_2dnav gmapping_demo.launch scan_topic:=/stable_scan

### To Save a Map
rosrun map_server map_saver -f "path/to/file/you/want/to/save"
