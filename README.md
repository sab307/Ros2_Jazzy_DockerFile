# Ros2_Jazzy_DockerFile

First run the following commands accoridngly. Before running docker please create a separate network.
```
docker network create ros2_zenoh_net
```

```
git clone this-repo
git submodule init
git submodule update
source /opt/ros/jazzy/setup.bash
sudo apt update
rosdep install -i -y --from-paths src --rosdistro jazzy
colcon build
```
This docker-network created would be utilized
by the Jazzy_Docker-compose repo and Iron as well.

P.S.

Just for more reference see the readme file in Humble and Iron repo, for how to add more camera's and modify the launch file.
```
sudo apt-get install net-tools && apt-get install iputils-ping
```