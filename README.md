<!-- DO NOT EDIT THIS FILE MANUALLY  -->
<!-- Please read the https://github.com/linuxserver/docker-steamos/blob/master/.github/CONTRIBUTING.md -->

[![linuxserver.io](https://raw.githubusercontent.com/linuxserver/docker-templates/master/linuxserver.io/img/linuxserver_medium.png)](https://linuxserver.io)

[![Blog](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Blog)](https://blog.linuxserver.io "all the things you can do with our containers including How-To guides, opinions and much more!")
[![Discord](https://img.shields.io/discord/354974912613449730.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Discord&logo=discord)](https://discord.gg/YWrKVTn "realtime support / chat with the community and the team.")
[![Discourse](https://img.shields.io/discourse/https/discourse.linuxserver.io/topics.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=discourse)](https://discourse.linuxserver.io "post on our community forum.")
[![Fleet](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Fleet)](https://fleet.linuxserver.io "an online web interface which displays all of our maintained images.")
[![GitHub](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub&logo=github)](https://github.com/linuxserver "view the source for all of our repositories.")
[![Open Collective](https://img.shields.io/opencollective/all/linuxserver.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Supporters&logo=open%20collective)](https://opencollective.com/linuxserver "please consider helping us by either donating or contributing to our budget")

The [LinuxServer.io](https://linuxserver.io) team brings you another container release featuring:

* regular and timely application updates
* easy user mappings (PGID, PUID)
* custom base image with s6 overlay
* weekly base OS updates with common layers across the entire LinuxServer.io ecosystem to minimise space usage, down time and bandwidth
* regular security updates

Find us at:

* [Blog](https://blog.linuxserver.io) - all the things you can do with our containers including How-To guides, opinions and much more!
* [Discord](https://discord.gg/YWrKVTn) - realtime support / chat with the community and the team.
* [Discourse](https://discourse.linuxserver.io) - post on our community forum.
* [Fleet](https://fleet.linuxserver.io) - an online web interface which displays all of our maintained images.
* [GitHub](https://github.com/linuxserver) - view the source for all of our repositories.
* [Open Collective](https://opencollective.com/linuxserver) - please consider helping us by either donating or contributing to our budget

# [linuxserver/steamos](https://github.com/linuxserver/docker-steamos)

[![Scarf.io pulls](https://scarf.sh/installs-badge/linuxserver-ci/linuxserver%2Fsteamos?color=94398d&label-color=555555&logo-color=ffffff&style=for-the-badge&package-type=docker)](https://scarf.sh/gateway/linuxserver-ci/docker/linuxserver%2Fsteamos)
[![GitHub Stars](https://img.shields.io/github/stars/linuxserver/docker-steamos.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-steamos)
[![GitHub Release](https://img.shields.io/github/release/linuxserver/docker-steamos.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-steamos/releases)
[![GitHub Package Repository](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub%20Package&logo=github)](https://github.com/linuxserver/docker-steamos/packages)
[![GitLab Container Registry](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitLab%20Registry&logo=gitlab)](https://gitlab.com/linuxserver.io/docker-steamos/container_registry)
[![Quay.io](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Quay.io)](https://quay.io/repository/linuxserver.io/steamos)
[![Docker Pulls](https://img.shields.io/docker/pulls/linuxserver/steamos.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=pulls&logo=docker)](https://hub.docker.com/r/linuxserver/steamos)
[![Docker Stars](https://img.shields.io/docker/stars/linuxserver/steamos.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=stars&logo=docker)](https://hub.docker.com/r/linuxserver/steamos)
[![Jenkins Build](https://img.shields.io/jenkins/build?labelColor=555555&logoColor=ffffff&style=for-the-badge&jobUrl=https%3A%2F%2Fci.linuxserver.io%2Fjob%2FDocker-Pipeline-Builders%2Fjob%2Fdocker-steamos%2Fjob%2Fmaster%2F&logo=jenkins)](https://ci.linuxserver.io/job/Docker-Pipeline-Builders/job/docker-steamos/job/master/)
[![LSIO CI](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=CI&query=CI&url=https%3A%2F%2Fci-tests.linuxserver.io%2Flinuxserver%2Fsteamos%2Flatest%2Fci-status.yml)](https://ci-tests.linuxserver.io/linuxserver/steamos/latest/index.html)

[SteamOS](https://www.steamdeck.com/) is an Arch based Linux distribution made by Valve Software. This container is a vanilla Arch install with Steam repositories added for software support. **This container will only work with modern AMD/Intel GPUs on a real Linux Host**

[![steamos](https://raw.githubusercontent.com/linuxserver/docker-templates/master/linuxserver.io/img/steamos-logo.png)](https://www.steamdeck.com/)

## Supported Architectures

We utilise the docker manifest for multi-platform awareness. More information is available from docker [here](https://github.com/docker/distribution/blob/master/docs/spec/manifest-v2-2.md#manifest-list) and our announcement [here](https://blog.linuxserver.io/2019/02/21/the-lsio-pipeline-project/).

Simply pulling `lscr.io/linuxserver/steamos:latest` should retrieve the correct image for your arch, but you can also pull specific arch images via tags.

The architectures supported by this image are:

| Architecture | Available | Tag |
| :----: | :----: | ---- |
| x86-64 | ✅ | amd64-\<version tag\> |
| arm64 | ❌ | |
| armhf | ❌ | |

## Application Setup

*This container is currently in a Beta state and is developing quickly, things will change constantly and it may crash or not function perfectly especially when mixing Steam remote play frame capture with the web based [KasmVNC](https://kasmweb.com/kasmvnc) frame capture*

**SteamOS is designed for specific AMD based hardware, this container will only work properly on a host with a modern AMD GPU or Intel ARC/iGPU**

The following limitations currently exist:
* You must run the desktop mode initially to login to Steam, then you can switch to `STARTUP=BIGPICTURE`
* Sunshine is available in both desktop mode (KDE) and BIGPICTURE, but gamepads using Sunshine does not currently work. 
* In Desktop mode most proton games will kill off kwin_x11 and in turn disable keyboard and gamepad input. For remote play in Desktop mode it is mostly Valve or Linux native titles that function properly.
* If games are not launching and are Windows based ensure you have forced a compatibility layer in it's settings to use Proton Experimental or Proton 8.
* BIGPICTURE STARTUP mode connecting via Sunshine will have much better game compatibility and generally be less buggy. Titles are running how the Steam Deck expects them to inside a gamescope renderer, outside of the lack of gamepads this works identically to a Deck.
* Sunshine auto discovery is not functional, you will need to manually enter the IP in your client. 
* Remote play does not function well in BIGPICTURE mode, this mode is optimized for a single resolution passed on boot using Sunshine.

To improve compatibility we ingest drivers from vanilla Arch repos, *but NVIDIA will never work*. This is a limitation of the [KasmVNC](https://kasmweb.com/kasmvnc) virtual framebuffer that we use as it only has logic for the [DRI3](https://en.wikipedia.org/wiki/Direct_Rendering_Infrastructure) framework which is not available for NVIDIA. We recommend using a modern RDNA AMD card or Intel ARC card, but lower end GPUs might work for some games we do bundle all the drivers that are possible to install.
Compatibility should be on par with the Steam Deck, if it is certified for the Deck it will run in our testing and the game should be fully playable.

The application can be accessed at:

* http://yourhost:3000/
* https://yourhost:3001/

### Options in all KasmVNC based GUI containers

This container is based on [Docker Baseimage KasmVNC](https://github.com/linuxserver/docker-baseimage-kasmvnc) which means there are additional environment variables and run configurations to enable or disable specific functionality.

#### Optional environment variables

| Variable | Description |
| :----: | --- |
| CUSTOM_PORT | Internal port the container listens on for http if it needs to be swapped from the default 3000. |
| CUSTOM_HTTPS_PORT | Internal port the container listens on for https if it needs to be swapped from the default 3001. |
| CUSTOM_USER | HTTP Basic auth username, abc is default. |
| PASSWORD | HTTP Basic auth password, abc is default. If unset there will be no auth |
| SUBFOLDER | Subfolder for the application if running a subfolder reverse proxy, need both slashes IE `/subfolder/` |
| TITLE | The page title displayed on the web browser, default "KasmVNC Client". |
| FM_HOME | This is the home directory (landing) for the file manager, default "/config". |
| DRINODE | If mounting in /dev/dri for [DRI3 GPU Acceleration](https://www.kasmweb.com/kasmvnc/docs/master/gpu_acceleration.html) allows you to specify the device to use IE `/dev/dri/renderD128` |

### Networking

**Windows users will need to disable their firewall for remote play to function in the default setup**

**The Steam Link application will only function in Host or Macvlan networking modes**

Steam network discovery in it's current state is pretty inflexible, to function locally it uses broadcast packets that cannot traverse subnets and this becomes a problem when using a Docker subnet. In the default configuration we recommend forwarding the ports and passing the underlying host's IP using the `HOST_IP` environment variable. When the container spins up it will set this IP as it's default route allowing remote play to function over a local network given the client does not have a firewall in the way blocking the traffic. If you never plan to use remote play or only plan on using it fully remote off your LAN through a Valve relay then you can essentially rip out all the logic for Steam port forwarding and passing the host ip to the container. 

Optimally [Macvlan](https://docs.docker.com/network/drivers/macvlan/) can be used to give this container a dedicated IP on your network and run closer to how a bridged VM would. This is the most compatible methodology and will avoid any potentially port conflicts. 

[Host Networking](https://docs.docker.com/network/drivers/host/) can also be used, but might run into a port conflict with what the container is trying to init and the underlying host.

### Gameplay

Keep in mind this container thinks it is a Steam Deck, games will be optimized for it's controller layout and video settings. To get a desktop Steam experience for remote play or testing there is a desktop shortcut provided `Steam Desktop Mode`.
Most games will tie themselves to the current desktop resolution as set when you connect to the web interface, a method for setting the resolution via the web interface is being worked on.
Authentication (not two factor) is not currently saved when closing and re-opening Steam for any reason when in Deck mode this is also being worked on. This means anytime you restart the container you will need to access the web interface and log back in.
It is possible to play games over KasmVNC, but it as a protocol is not currently optimized for gaming. You will experience more frame skipping and latency as compared to Steam remote play.

## Usage

Here are some example snippets to help you get started creating a container.

### docker-compose (recommended, [click here for more info](https://docs.linuxserver.io/general/docker-compose))

```yaml
---
version: "2.1"
services:
  steamos:
    image: lscr.io/linuxserver/steamos:latest
    container_name: steamos
    hostname: hostname #optional
    cap_add:
      - NET_ADMIN
    security_opt:
      - seccomp:unconfined
      - apparmor:unconfined #optional
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=Etc/UTC
      - DRINODE=/dev/dri/renderD128
      - HOST_IP=192.168.100.10 #optional
      - STARTUP=KDE #optional
      - RESOLUTION=1920x1080 #optional
    volumes:
      - /path/to/config:/config
      - /dev/input:/dev/input #optional
      - /run/udev/data:/run/udev/data #optional
    ports:
      - 3000:3000
      - 3001:3001
      - 27031-27036:27031-27036/udp #optional
      - 27031-27036:27031-27036 #optional
      - 47984-47990:47984-47990 #optional
      - 48010:48010:48010:48010 #optional
      - 47998-48000:47998-48000/udp #optional
    devices:
      - /dev/dri:/dev/dri
    shm_size: "1gb"
    restart: unless-stopped
```

### docker cli ([click here for more info](https://docs.docker.com/engine/reference/commandline/cli/))

```bash
docker run -d \
  --name=steamos \
  --hostname=hostname `#optional` \
  --cap-add=NET_ADMIN \
  --security-opt seccomp=unconfined \
  --security-opt apparmor=unconfined `#optional` \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Etc/UTC \
  -e DRINODE=/dev/dri/renderD128 \
  -e HOST_IP=192.168.100.10 `#optional` \
  -e STARTUP=KDE `#optional` \
  -e RESOLUTION=1920x1080 `#optional` \
  -p 3000:3000 \
  -p 3001:3001 \
  -p 27031-27036:27031-27036/udp `#optional` \
  -p 27031-27036:27031-27036 `#optional` \
  -p 47984-47990:47984-47990 `#optional` \
  -p 48010:48010:48010:48010 `#optional` \
  -p 47998-48000:47998-48000/udp `#optional` \
  -v /path/to/config:/config \
  -v /dev/input:/dev/input `#optional` \
  -v /run/udev/data:/run/udev/data `#optional` \
  --device /dev/dri:/dev/dri \
  --shm-size="1gb" \
  --restart unless-stopped \
  lscr.io/linuxserver/steamos:latest

```

## Parameters

Container images are configured using parameters passed at runtime (such as those above). These parameters are separated by a colon and indicate `<external>:<internal>` respectively. For example, `-p 8080:80` would expose port `80` from inside the container to be accessible from the host's IP on port `8080` outside the container.

| Parameter | Function |
| :----: | --- |
| `--hostname=` | Specify the hostname of the host, this is useful for keeping a persistent hostname between upgrades and identifying the server in the remote play Steam Client. |
| `-p 3000` | SteamOS desktop gui. |
| `-p 3001` | HTTPS SteamOS desktop gui. |
| `-p 27031-27036/udp` | Steam Remote Play Ports (UDP). |
| `-p 27031-27036` | Steam Remote Play Ports (TCP). |
| `-p 47984-47990` | Sunshine Ports (TCP). |
| `-p 48010:48010` | Sunshine Ports (TCP). |
| `-p 47998-48000/udp` | Sunshine Ports (UDP). |
| `-e PUID=1000` | for UserID - see below for explanation |
| `-e PGID=1000` | for GroupID - see below for explanation |
| `-e TZ=Etc/UTC` | specify a timezone to use, see this [list](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List). |
| `-e DRINODE=/dev/dri/renderD128` | Specify the render device (GPU) for the contianer to use. |
| `-e HOST_IP=192.168.100.10` | Specify the IP of the host, needed for LAN Remote Play. |
| `-e STARTUP=KDE` | KDE to boot into desktop mode, BIGPICTURE to boot into gamescope. |
| `-e RESOLUTION=1920x1080` | When booting into BIGPICTURE mode the screen resolution will be bound to this value. |
| `-v /config` | Users home directory in the container, stores all files and games. |
| `-v /dev/input` | Optional for gamepad support. *Only working for Steam Remote Play |
| `-v /run/udev/data` | Optional for gamepad support. *Only working for Steam Remote Play |
| `--device /dev/dri` | Video card passthrough to Steam. |
| `--shm-size=` | This is needed for the steam browser to function properly. |
| `--security-opt seccomp=unconfined` | This is needed to allow kernel syscalls made by Steam. |
| `--security-opt apparmor=unconfined` | For Debian/Ubuntu hosts Steam needs elevated perms that AppArmor blocks. |

### Portainer notice

This image utilises `cap_add` or `sysctl` to work properly. This is not implemented properly in some versions of Portainer, thus this image may not work if deployed through Portainer.

## Environment variables from files (Docker secrets)

You can set any environment variable from a file by using a special prepend `FILE__`.

As an example:

```bash
-e FILE__PASSWORD=/run/secrets/mysecretpassword
```

Will set the environment variable `PASSWORD` based on the contents of the `/run/secrets/mysecretpassword` file.

## Umask for running applications

For all of our images we provide the ability to override the default umask settings for services started within the containers using the optional `-e UMASK=022` setting.
Keep in mind umask is not chmod it subtracts from permissions based on it's value it does not add. Please read up [here](https://en.wikipedia.org/wiki/Umask) before asking for support.

## User / Group Identifiers

When using volumes (`-v` flags) permissions issues can arise between the host OS and the container, we avoid this issue by allowing you to specify the user `PUID` and group `PGID`.

Ensure any volume directories on the host are owned by the same user you specify and any permissions issues will vanish like magic.

In this instance `PUID=1000` and `PGID=1000`, to find yours use `id user` as below:

```bash
  $ id username
    uid=1000(dockeruser) gid=1000(dockergroup) groups=1000(dockergroup)
```

## Docker Mods

[![Docker Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=steamos&query=%24.mods%5B%27steamos%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=steamos "view available mods for this container.") [![Docker Universal Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=universal&query=%24.mods%5B%27universal%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=universal "view available universal mods.")

We publish various [Docker Mods](https://github.com/linuxserver/docker-mods) to enable additional functionality within the containers. The list of Mods available for this image (if any) as well as universal mods that can be applied to any one of our images can be accessed via the dynamic badges above.

## Support Info

* Shell access whilst the container is running: `docker exec -it steamos /bin/bash`
* To monitor the logs of the container in realtime: `docker logs -f steamos`
* container version number
  * `docker inspect -f '{{ index .Config.Labels "build_version" }}' steamos`
* image version number
  * `docker inspect -f '{{ index .Config.Labels "build_version" }}' lscr.io/linuxserver/steamos:latest`

## Updating Info

Most of our images are static, versioned, and require an image update and container recreation to update the app inside. With some exceptions (ie. nextcloud, plex), we do not recommend or support updating apps inside the container. Please consult the [Application Setup](#application-setup) section above to see if it is recommended for the image.

Below are the instructions for updating containers:

### Via Docker Compose

* Update all images: `docker-compose pull`
  * or update a single image: `docker-compose pull steamos`
* Let compose update all containers as necessary: `docker-compose up -d`
  * or update a single container: `docker-compose up -d steamos`
* You can also remove the old dangling images: `docker image prune`

### Via Docker Run

* Update the image: `docker pull lscr.io/linuxserver/steamos:latest`
* Stop the running container: `docker stop steamos`
* Delete the container: `docker rm steamos`
* Recreate a new container with the same docker run parameters as instructed above (if mapped correctly to a host folder, your `/config` folder and settings will be preserved)
* You can also remove the old dangling images: `docker image prune`

### Via Watchtower auto-updater (only use if you don't remember the original parameters)

* Pull the latest image at its tag and replace it with the same env variables in one run:

  ```bash
  docker run --rm \
  -v /var/run/docker.sock:/var/run/docker.sock \
  containrrr/watchtower \
  --run-once steamos
  ```

* You can also remove the old dangling images: `docker image prune`

**Note:** We do not endorse the use of Watchtower as a solution to automated updates of existing Docker containers. In fact we generally discourage automated updates. However, this is a useful tool for one-time manual updates of containers where you have forgotten the original parameters. In the long term, we highly recommend using [Docker Compose](https://docs.linuxserver.io/general/docker-compose).

### Image Update Notifications - Diun (Docker Image Update Notifier)

* We recommend [Diun](https://crazymax.dev/diun/) for update notifications. Other tools that automatically update containers unattended are not recommended or supported.

## Building locally

If you want to make local modifications to these images for development purposes or just to customize the logic:

```bash
git clone https://github.com/linuxserver/docker-steamos.git
cd docker-steamos
docker build \
  --no-cache \
  --pull \
  -t lscr.io/linuxserver/steamos:latest .
```

The ARM variants can be built on x86_64 hardware using `multiarch/qemu-user-static`

```bash
docker run --rm --privileged multiarch/qemu-user-static:register --reset
```

Once registered you can define the dockerfile to use with `-f Dockerfile.aarch64`.

## Versions

* **04.07.23:** - Initial release.
