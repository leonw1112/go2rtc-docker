# go2rtc-docker
Docker Container to run and start go2rtc automatically

- To run automatically on startup:

### Many modern Linux distributions use systemd to manage which services start when the system boots. On Debian and Ubuntu, the Docker service starts on boot by default. To automatically start Docker and containerd on boot for other Linux distributions using systemd, run the following commands:

 ``sudo systemctl enable docker.service``

 ``sudo systemctl enable containerd.service``

### To stop this behavior, use disable instead

 ``sudo systemctl disable docker.service``

 ``sudo systemctl disable containerd.service``

- If you need to add an HTTP proxy, set a different directory or partition for the Docker runtime files, or make other customizations, see customize your systemd Docker daemon options.

-  When changing something in the docker-compose config, remember to delete the old container and change the credentials in the go2rtc.yaml, this is an example for the tapo cameras. see the credit link below for more information.

#### Credits: https://github.com/AlexxIT/go2rtc
