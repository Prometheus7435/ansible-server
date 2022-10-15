# ansible-server
My ansible setup to initial creation of a server to fit my needs. This is very heavily inspired from [ansible-nas](https://github.com/davestephens/ansible-nas) and there will be much overlap as I am very new to Ansible.

# Services
These are mostly a copy from Ansible-NAS, but with my additions at the bottom. Eventually, this list'll get paired down as there are some duplicates and services I don't know if I want. The ones I added are from parusing [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) and the [Self-Hosted podcast](https://selfhosted.show/). Some of these services will work best as seperate virtual machines, but that'll be for another day.
* [Airsonic](https://airsonic.github.io/) - catalog and stream music
* [Bazarr](https://github.com/morpheus65535/bazarr) - companion to Radarr and Sonarr for downloading subtitles
* [Bitwarden_rs](https://github.com/dani-garcia/bitwarden_rs) - Self-Hosting port of password manager
* [Booksonic](https://booksonic.org/) - The selfhosted audiobook server
* [Calibre-web](https://github.com/janeczku/calibre-web) - Provides a clean interface for browsing, reading and downloading eBooks using an existing Calibre database.
* [Cloudflare DDNS](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns/) - automatically update Cloudflare with your IP address
* [CouchPotato](https://couchpota.to/) - for downloading and managing movies
* [Dashy](https://dashy.to/) - A self-hosted startpage for your server. Easy to use visual editor, status checking, widgets, themes and tons more!
* [Deluge](https://dev.deluge-torrent.org/) - A lightweight, Free Software, cross-platform BitTorrent client.
* [Duplicacy](https://duplicacy.com/) - A web UI for the Duplicacy cloud backup program, which provides lock-free deduplication backups to multiple providers
* [Duplicati](https://www.duplicati.com/) - for backing up your stuff
* [Emby](https://emby.media/) - Media streaming and management
* [ESPHome](https://esphome.io/) - ESP8266/ESP32 programming and management for home automation
* [Firefly III](https://firefly-iii.org/) - Free and open source personal finance manager
* [Fresh RSS](https://freshrss.org/) - Self-hosted RSS feed aggregator like Leed or Kriss Feed
* [Gitea](https://gitea.io/en-us/) - Simple self-hosted GitHub clone (debating between this and GitLab. Don't need all the features of GitLab, but it'd be nice to have in case)
* [GitLab](https://about.gitlab.com/features/) - Self-hosted GitHub clone of the highest order
* [Glances](https://nicolargo.github.io/glances/) - for seeing the state of your system via a web browser
* [Gotify](https://gotify.net/) - Self-hosted server for sending push notifications
* [Grafana](https://grafana.com/) - Query, visualize, alert on, and understand your data no matter where it’s stored (via stats role).
* [Guacamole](https://guacamole.apache.org/) - Web based remote desktop gateway, supports VNC, RDP and SSH
* [healthchecks.io](https://healthchecks.io/) - Ensure your NAS is online and get notified otherwise
* [Heimdall](https://heimdall.site/) - Home server dashboard
* [Home Assistant](https://www.home-assistant.io) - Open source home automation (this will be turned into a VM. You don't get all the features unless you use their VM)
* [Jackett](https://github.com/Jackett/Jackett) - API Support for your favorite torrent trackers
* [Jellyfin](https://jellyfin.github.io) - The Free Software Media System
* [Joomla](https://www.joomla.org/) - Open source content management system
* [Komga](https://komga.org/) - a media server for your comics, mangas, BDs and magazines
* [Lidarr](https://github.com/lidarr/Lidarr) - Music collection manager for Usenet and BitTorrent users
* [Mealie](https://hay-kot.github.io/mealie/) - A self-hosted recipe manager and meal planner
* [MiniDLNA](https://sourceforge.net/projects/minidlna/) - simple media server which is fully compliant with DLNA/UPnP-AV clients
* [Miniflux](https://miniflux.app/) - An RSS news reader
* [Mosquitto](https://mosquitto.org) - An open source MQTT broker (may or may not be needed as I'm using HomeAssistant)
* [Mylar](https://github.com/evilhero/mylar) - An automated Comic Book downloader (cbr/cbz) for use with SABnzbd, NZBGet and torrents
* [MyMediaForAlexa](https://www.mymediaalexa.com/) - Lets you stream your music collection to your alexa device
* [navidrome](https://www.navidrome.org/) - Modern Music Server and Streamer compatible with Subsonic/Airsonic
* [netboot.xyz](https://netboot.xyz/) - a PXE boot server
* [Netdata](https://my-netdata.io/) - An extremely comprehensive system monitoring solution
* [Nextcloud](https://nextcloud.com/) - A self-hosted Dropbox alternative
* [NZBget](https://nzbget.net/) - The most efficient usenet downloader
* [Ombi](https://ombi.io/) - web application that automatically gives your users the ability to request content
* [Organizr](https://organizr.app/) - ORGANIZR aims to be your one stop shop for your Servers Frontend.
* [overseerr](https://docs.overseerr.dev) - open source software application for managing requests for your media library
* [Paperless_ng](https://github.com/jonaswinkler/paperless-ng) - Scan, index and archive all your physical documents
* [Plex](https://www.plex.tv/) - Plex Media Server
* [Portainer](https://portainer.io/) - for managing Docker and running custom images
* [Prometheus](https://prometheus.io/) - Time series database and monitoring system (via stats role).
* [Prowlarr](https://github.com/Prowlarr/Prowlarr) - Indexer aggregator for Sonarr, Radarr, Lidarr, etc.
* [pyLoad](https://pyload.net/) - A download manager with a friendly web-interface
* [Radarr](https://radarr.video/) - for organising and downloading movies
* [Route53 DDNS](https://crazymax.dev/ddns-route53/) - Automatically update AWS Route53 with your IP address (do I want anything Amazon?)
* [RSS-Bridge](https://rss-bridge.github.io/rss-bridge/) - The RSS feed for websites missing it
* [Sickchill](https://sickchill.github.io/) - for managing TV episodes
* [Sonarr](https://sonarr.tv/) - for downloading and managing TV episodes
* [Syncthing](https://syncthing.net/) - sync directories with another device
* [Traefik](https://traefik.io/) - Web proxy and SSL certificate manager
* [Transmission](https://transmissionbt.com/) - BitTorrent client (with OpenVPN if you have a supported VPN provider)
* [Ubooquity](http://vaemendis.net/ubooquity/) - Book and comic server
* [uTorrent](https://www.utorrent.com/) - The best torrent downloading app for beginners
* [Virtual Desktop](https://github.com/RattyDAVE/docker-ubuntu-xrdp-mate-custom) - A virtual desktop running on your NAS.
* [Wallabag](https://wallabag.org/) - Save and classify articles. Read them later.
* [Watchtower](https://github.com/v2tec/watchtower) - Monitor your Docker containers and update them if a new version is available (testing)
* [YouTubeDL-Material](https://github.com/Tzahi12345/YoutubeDL-Material) - Self-hosted YouTube downloader built on Material Design
* Exadel Compare Face
* Hagium
* open library
* Medusa
* Tube Archivish
* utask
* Baihal
* FreePBX (prob on seperate server, but want to test it out before deploying - if I ever do)
* Stump
* Kavita
* Full-Text RSS
* Audio bookshelf
* 2F Auth
* Monica
* Ombi
* Teleport
* Tandoor Recipes
* Media Wiki (when doing anything, over do it. Or at least that's my habit)

# Assumptions
Since you can't netboot a complete Ansible install (or could you? I should look that up), I've made some assumptions on the system this'll be implemented in.

## OS
The OS (as of now) is whatever the most current Ubuntu LTS is. I'm not so much a fan of all the snap stuff they're putting in, so this might change to OpenSUSE or CENTOS Stream in the future.

## File System
ZFS everywhere. Okay, maybe not for the OS just yet. But everywhere else that data'll be, it will have ZFS as the file system. There will be subvolumes that will be created in this setup, so the base setup of the pool is all that's required of the user.
