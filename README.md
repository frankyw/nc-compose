
## frankyw/nc-compose

This is a repository to version control a friend's server setup.

### Docker Containers

The following containers are being run:

* [linuxserver/wireguard](https://hub.docker.com/r/linuxserver/wireguard) - LinuxServer.io Wireguard container, which replaced OpenVPN built into the previous Tranmission container (huge difference!)
* [wiserain/flexget](https://hub.docker.com/r/wiserain/flexget/) - A small and well-maintained FlexGet container that includes the plugins needed. Uses the Wireguard container for networking.
* [linuxserver/transmission](https://hub.docker.com/r/linuxserver/transmission/) - Transmission from LinuxServer.io, uses the Wireguard container for networking.
* [rednoah/filebot:node](https://hub.docker.com/r/rednoah/filebot/) - Official Filebot container, used for automated media management.
* [traefik:latest](https://hub.docker.com/_/traefik) - Official Traefik container, reverse proxy to expose services over TLS using Let's Encrypt in a far simpler way than nginx (imo). 
* [portainer/portainer](https://hub.docker.com/r/portainer/portainer) - Official Portainer image, used for docker cluster management.
* [emby/embyserver:beta](https://hub.docker.com/r/emby/embyserver) - Official Emby beta container.
* [containrrr/watchtower](https://hub.docker.com/r/containrrr/watchtower) - Official Watchtower image to update containers.
* [linuxserver/duplicati](https://hub.docker.com/r/linuxserver/duplicati) - A Duplicati container, flexible and easy to use system which backs up files to the cloud.
* [cloudflare-ddns](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns) - Keep that IP address up-to-date!
* [home-assistant](https://www.home-assistant.io/installation/alternative#docker-compose) - Home Assistant for home automation.

## Configuration

I am using a Docker .env file, which contains all the variables found in the docker-compose.yml