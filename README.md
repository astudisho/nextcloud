# Nextcloud All-in-One (AIO) Setup

This project uses Docker Compose to deploy Nextcloud All-in-One (AIO), a convenient way to run Nextcloud with all its essential components in Docker containers.

## Table of Contents

* [Prerequisites](#prerequisites)
* [Getting Started](#getting-started)
    * [1. Clone the Repository (or create `docker-compose.yml`)](#1-clone-the-repository-or-create-docker-composeyml)
    * [2. Configure the `docker-compose.yml` (Optional but Recommended)](#2-configure-the-docker-composeyml-optional-but-recommended)
    * [3. Start Nextcloud AIO](#3-start-nextcloud-aio)
    * [4. Access Nextcloud AIO Interface](#4-access-nextcloud-aio-interface)
* [Important Considerations](#important-considerations)
    * [Data Directory Location](#data-directory-location)
    * [Memory Limit](#memory-limit)
    * [Port Mapping](#port-mapping)
    * [Reverse Proxy / SSL](#reverse-proxy--ssl)
    * [Backups](#backups)
    * [Permissions](#permissions)
* [Troubleshooting](#troubleshooting)
* [Credits](#credits)

## Prerequisites

Before you begin, ensure you have the following installed on your system (e.g., Raspberry Pi, Linux server):

* **Docker:** [Installation Guide](https://docs.docker.com/engine/install/)
* **Docker Compose:** Usually comes with Docker Desktop, or can be installed separately for Linux systems (e.g., `sudo apt install docker-compose-plugin` or `sudo pip install docker-compose`).
* **Minimum Hardware:** Nextcloud AIO has specific resource requirements. While it can run on a Raspberry Pi, ensure your model has sufficient RAM (Raspberry Pi 4 with at least 4GB RAM is recommended for a smooth experience). Refer to the [Nextcloud AIO GitHub](https://github.com/nextcloud/all-in-one) for detailed recommendations.

## Getting Started

Follow these steps to get your Nextcloud AIO instance up and running.

### 1. Clone the Repository (or create `docker-compose.yml`)

If you received this `docker-compose.yml` file, you can simply place it in a directory on your server.

```bash
# If you have a Git repository for this project:
git clone <your-repo-url>
cd <your-repo-name>

# Otherwise, create a directory and paste the docker-compose.yml content:
mkdir nextcloud-aio
cd nextcloud-aio
# Create a file named docker-compose.yml and paste the provided content into it.
nano docker-compose.yml # or your preferred text editor