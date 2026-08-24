# Ubuntu Docker Installation

Follow these steps to install Docker on Ubuntu.

## 1. Update the system packages

Run the following command if you want to update your system packages:

```bash
sudo apt update && sudo apt upgrade -y
```

> This command is optional.

## 2. Download the Docker installation script

```bash
curl -fsSL https://get.docker.com -o get-docker.sh
```

## 3. Install Docker

```bash
sudo sh get-docker.sh
```

## 4. Add your user to the Docker group

```bash
sudo usermod -aG docker $USER && newgrp docker
```

## 5. Verify the installation

Run the following command to check whether Docker was installed correctly:

```bash
docker run hello-world
```

This will download a test container and confirm that Docker is working properly.
