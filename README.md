# alafia-neurodesktop

## Description

Alafia-specific deployment of [neurodesktop](https://www.neurodesk.org/docs/getting-started/neurodesktop/) based on [the official Docker image](https://hub.docker.com/r/vnmd/neurodesktop). This app is run in the browser. It can be accessed by navigating to https://neurodesktop.alafia, clicking the link in https://home.alafia, or by running the application launcher from the desktop. Neurodesktop provides many containerized neuroimaging apps.

## Usage

Meant to be used as a submodule in [alafia-apps](https://github.com/Alafia-Ai/alafia-apps).

`Makefile` can be manually invoked with the following options:

- `make` or `make build`: Locally build the Docker image
- `make install`: Install the files in the `deploy/` directory, and if relevant, install systemd service files and modify `/etc/hosts/`
- `make uninstall`: Removes all installed files, and if relevant, removes systemd services and resets `/etc/hosts/` 
