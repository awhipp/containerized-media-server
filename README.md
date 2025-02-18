# Containerized Media Server

Welcome to the Containerized Media Server repository! This project is designed to help you quickly set up your own media server using the following applications:

- **Plex**: A media server that organizes your media and streams it to any device.
- **Sonarr**: A TV show collection manager.
- **Radarr**: A movie collection manager.
- **Prowlarr**: An indexer manager/proxy for Sonarr, Radarr, and other applications.
- **Overseerr**: A request management and media discovery tool for your media server.

## Architecture

![Architecture](./diagram.drawio.svg)

## Requirements

1. Docker
2. Nvidia Container Kit (for GPU support) or WSL2 (windows for GPU support)
3. A media library

## Getting Started

To get started with setting up your media server, follow these steps:

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/containerized-media-server.git
    cd containerized-media-server
    ```

2. **Configure Environment Variables**
    - Create a `.env` file in the root directory and add the necessary environment variables for each application.

3. **Run Docker Compose**
    - Use Docker Compose to set up and run all the services.

    ```sh
    docker-compose up -d
    ```

4. **Access Your Applications**
    - Plex: `http://localhost:32400`
    - Sonarr: `http://localhost:8989`
    - Radarr: `http://localhost:7878`
    - Prowlarr: `http://localhost:9696`

5. To update images (example with plex)

    ```sh
    docker pull linuxserver/plex:latest
    docker stop plex
    docker rm plex
    docker compose up -d plex
    ```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

Enjoy your new media server setup!
