
## frankyw/nc-compose

This is a repository to version control a friend's server setup.

### Docker Containers

The following containers are being run:  

### Arr Stack

* [hotio/sonarr](https://hotio.dev/containers/sonarr/) - Management and automation of TV Show downloading.
* [hotio/radarr](https://hotio.dev/containers/radarr/) - Management and automation of Movie downloading.
* [hotio/unpackerr](https://hotio.dev/containers/unpackerr/) - Very nice container to handle compressed archives cleanly.
* [hotio/jackett](https://hotio.dev/containers/jackett/) - API Support for my trackers, to provide content to Sonarr and Radarr.
* [autobrr/autobrr](https://autobrr.com/installation/docker) - Get releases within seconds from IRC Announce Channels, and pass to Sonarr.

### Other

* [traefik:latest](https://hub.docker.com/_/traefik) - Official Traefik container, reverse proxy to expose services over TLS using Let's Encrypt in a far simpler way than nginx (imo). 
* [linuxserver/qbittorrent](https://docs.linuxserver.io/images/docker-qbittorrent/) - Got fed up [Transmission 4.0 slow speeds](https://github.com/transmission/transmission/issues/5261), and switched to qBittorent.
* [linuxserver/duplicati](https://hub.docker.com/r/linuxserver/duplicati) - A Duplicati container, flexible and easy to use system which backs up files to the cloud.
* [linuxserver/plex](https://docs.linuxserver.io/images/docker-plex) - Plex for PS5 AR Glasses.
* [bobokun/qbit_manage](https://hub.docker.com/r/bobokun/qbit_manage) - Very helpful program to cleanup qBitorrent torrents.
* [qmcgaw/gluetun](https://hub.docker.com/r/qmcgaw/gluetun) - Great VPN container that supports easy Wireguard config.
* [portainer/portainer](https://hub.docker.com/r/portainer/portainer) - Official Portainer image, used for docker cluster management.
* [emby/embyserver:beta](https://hub.docker.com/r/emby/embyserver) - Official Emby beta container.
* [containrrr/watchtower](https://hub.docker.com/r/containrrr/watchtower) - Official Watchtower image to update containers.
* [cloudflare-ddns](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns) - Keep that IP address up-to-date!
* [home-assistant](https://www.home-assistant.io/installation/alternative#docker-compose) - Home Assistant for home automation.

## Configuration

This config uses a docker .env file, which contains all the variables found in the docker-compose.yml