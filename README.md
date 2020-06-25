
## frankyw/nc-compose

This is a repository to version control a friend's server setup.

### Docker Containers

The following containers are being run:

* [wiserain/flexget](https://hub.docker.com/r/wiserain/flexget/) - A small and well-maintained FlexGet container that includes the plugins needed.
* [haugene/transmission-openvpn]([https://hub.docker.com/r/haugene/transmission-openvpn](https://hub.docker.com/r/haugene/transmission-openvpn)) - Transmission with OpenVPN, which is suitable for use in the UK where literally everything is monitored and blocked. Also provides Tinyproxy for FlexGet to use.
* [rednoah/filebot:node](https://hub.docker.com/r/rednoah/filebot/) - Official Filebot container, used for automated media management.
* [traefik:latest](https://hub.docker.com/_/traefik) - Official Traefik container, reverse proxy to expose services over TLS using Let's Encrypt in a far simpler way than nginx. 
* [portainer/portainer](https://hub.docker.com/r/portainer/portainer) - Official Portainer image, docker cluster management.
* [emby/embyserver:beta](https://hub.docker.com/r/emby/embyserver) - Official Emby beta container.
* [containrrr/watchtower](https://hub.docker.com/r/containrrr/watchtower) - Official Watchtower image to update all containers.
* [linuxserver/duplicati]([https://hub.docker.com/r/linuxserver/duplicati](https://hub.docker.com/r/linuxserver/duplicati)) - A Duplicati container, a very flexible and easy to use system which provides the ability to backup files to the cloud.
* [cloudflare-ddns]([https://hub.docker.com/r/joshuaavalon/cloudflare-ddns](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns)) - Keep that IP address up-to-date!

## Configuration

I am using a Docker .env file, which contains all the variables found in the docker-compose.yml