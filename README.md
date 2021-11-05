

# Personal Server
***Author: Finn Morris
Created: 10/03/21
Modified: 05/11/21***


# Description:
Multi-purpose server running docker containers and constant C++ programs
### Hardware: 
- HP Compaq Elite 8300 Desktop 
- Intel i7 3770 3.40Ghz 
- 8Gb Ram 
- 500Gb HDD
- 160Gb HDD
- 1Tb External SSD
### Software:
- OpenMediaVault v5.6
- Docker
 
# Purpose:

### Nextcloud
Container to run nextcloud self hosted service, a cloud based file storage system.

### Octoprint
Container to run 3D printing communcation software to manage files and interactions with 3D printers.

### HomeAssistant
Container to run HomeAssistant, an open source home automation control platform.

### Mosquitto
Container to run Eclipse mosquitto, an open source MQTT broker to bridge communication from MQTT devices and homeassistant.

### Deconz
Container to run zigbee gateway program Deconz, an hub for all zigbee enabled devices to communicate to.

### Portainer
Container to run program Portainer, a container management application.

~~### DuckDNS
A container to run a DNS solution that automatically assigns SSL certificates and redirects incoming traffic through specified ports.~~
### Nginx Proxy Manager
Previously a SWAG instance was used to process SSL and Reverse Proxy however multiple config files and docker-compose files lead to complications that were simplified with NGINX Proxy Manager, a UI based application that handles everything SWAG does in a single docker container with no extra config files. 
The description of previously used SWAG is below:
Swag instance is a fantasic package containing NGINX reverse proxy and SSL encryption in one. This used with Cloudflares dynamic DNS assignment createds a protected, dedicated adress for each docker container.
eg: homeassistant.mydomain.com, nextcloud.mydomain.com..

### Kinect Body Tracker
A C++ program based on NiTE examples from OpenKinect v2 that uses room positioning to execute HTTP POST commands
