# Ansible Docker Image

This repository contains the CI pipeline for building an Ansible Docker image. It also provides a repository on ghcr.io for your DevOps usage. Supported architectures are `amd64`, `arm64`.

## Getting Started

I don't recommend using the source code in this repository directly. Instead, you should use the built Docker image from the ghcr.io repository. The image is built automatically on every commit to the main branch and pushed to the ghcr.io repository.

To use the Ansible Docker image in your DevOps workflows, pull the image from the ghcr.io repository using the following command:

```bash
docker pull ghcr.io/jyje/ansible
```

## CI Pipeline

The CI pipeline in this repository is responsible for building the Ansible Docker image. It can be customized to fit your specific requirements. The pipeline is triggered on every commit to the main branch and automatically builds and pushes the Docker image to the ghcr.io repository.

## Usage

To use the Ansible Docker image in your DevOps workflows, follow these steps:

1. Pull the Docker image from the ghcr.io repository.

```bash
docker pull ghcr.io/jyje/ansible
```
2. Run the Docker container using the pulled image.
3. Execute your Ansible playbooks and tasks inside the running container.

### Using Specific Version

You can use a specific version of the Ansible Docker image by specifying the version tag. For example, to use version `9.2.0`, use the following command:

```bash
docker pull ghcr.io/jyje/ansible:9.2.0
```



# Preinstalled Utilities
This image provides following utilities preinstalled:
```
- ansible
- python
- pip

- curl
- git
- jq
- openssh-client
- vim
- wget
```
