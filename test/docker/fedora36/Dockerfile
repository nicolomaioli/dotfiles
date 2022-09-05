FROM fedora:36

ARG username
ARG password

RUN dnf install -y \
		ansible \
		curl \
		wget \
		git \
		openssl

# Create a non-root user with sudo privileges
RUN useradd -m -p $(openssl passwd -1 ${password}) -s /bin/bash -G wheel ${username}
USER docker
WORKDIR /home/docker
