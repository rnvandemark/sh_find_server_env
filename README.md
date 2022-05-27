# sh_find_server_env

## Set up Docker and the FIND3 server image

```
curl -sSL https://get.docker.com | sh
docker pull schollz/find3
```

## Build instructions for our select ROS2 repos

```
sudo apt update && sudo apt install -y \
  httpie \
  libjsoncpp-dev

mkdir -p /path/to/your_ws/src
cd /path/to/your_ws
rosinstall src /path/to/sh_find_server_env/sh_find_server.rosinstall
```
