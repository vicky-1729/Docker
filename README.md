# Docker

## Docker Installation Steps (RHEL/CentOS)

1. **Install required plugins:**
	```sh
	sudo dnf -y install dnf-plugins-core
	```

2. **Add Docker repository:**
	```sh
	sudo dnf config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo
	```

3. **Install Docker packages:**
	```sh
	sudo dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
	```

4. **Add your user to the Docker group (to run Docker as a non-root user):**
	```sh
	sudo usermod -aG docker ec2-user
	```

> **Note:** After adding your user to the Docker group, log out and log back in for the changes to take effect.