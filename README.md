Dockerfile for Dubian stretch with systemd


## Usage

You can run container with:
```bash
docker run -dt -v /sys/fs/cgroup:/sys/fs/cgroup:ro --tmpfs /run --tmpfs /run/lock --security-opt seccomp=unconfined  ultransible/debian_9_systemd name_container 
```
## Build the container

If you want to re-build the container, you have to clone the repo and trigger the building:
```bash
git clone  https://github.com/ultransible/debian_9_systemd.git
cd debian_9_systemd
docker build .
