# hs-config

This repository contains configuration files for Dockerized Headscale, a self-hosted implementation of Tailscale control server.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Overview

Headscale is an open-source, self-hosted implementation of the Tailscale control server. This repository provides the necessary configuration files to set up and run Headscale in a Dockerized environment, making it easy to deploy and manage.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/saahirlol/hs-config.git
    ```
2. Navigate to the directory:
    ```bash
    cd hs-config/server
    ```
3. Build and run the Docker containers:
    ```bash
    docker-compose up --build
    ```

## Usage

After installation, Headscale will be running in Docker containers. You can interact with the Headscale server using the provided configuration files.

### Common Commands

- To start the containers:
    ```bash
    docker-compose up
    ```

- To stop the containers:
    ```bash
    docker-compose down
    ```

- To view logs:
    ```bash
    docker-compose logs -f
    ```

## Configuration

Configuration files are located in the `config` directory. You can customize the Headscale settings by editing the following files:

- `config.yaml`: Main configuration file for Headscale.
- `docker-compose.yml`: Docker Compose file to manage Docker containers.

### Customizing `config.yaml`

To change the settings for your Headscale instance, open the `config.yaml` file and modify the parameters as needed. For example, to change the server address:
```yaml
server:
  addr: "your-server-address:port"
```

### Customizing `docker-compose.yml`

To adjust Docker settings, such as container names or volumes, edit the `docker-compose.yml` file.

## Contributing

We welcome contributions from the community! If you'd like to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix:
    ```bash
    git checkout -b feature-name
    ```
3. Make your changes and commit them with clear and concise messages.
4. Push your changes to your forked repository:
    ```bash
    git push origin feature-name
    ```
5. Open a pull request with a description of your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

If you encounter any issues or have suggestions for improvements, feel free to open an issue on the [GitHub repository](https://github.com/saahirlol/hs-config/issues). Happy self-hosting!
