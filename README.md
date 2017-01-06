# knxd-build-docker-rpi
Docker image to build knxd with all required dependencies on a raspberry pi. Tested on a raspi3/Jessie.

The resulting packages are available in the 'packages' directory.
```
sudo docker build -t knxd-build-docker-rpi .
mkdir packages
sudo docker run -v `realpath packages`:/packages knxd-build-docker-rpi
```
