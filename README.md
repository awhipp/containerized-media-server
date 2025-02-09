# Whipp Media Server

Welcome to the Whipp Media Server repository! This project is designed to help you quickly set up your own media server using the following applications:

- **Plex**: A media server that organizes your media and streams it to any device.
- **Sonarr**: A PVR for Usenet and BitTorrent users to manage TV shows.
- **Radarr**: A movie collection manager for Usenet and BitTorrent users.
- **Prowlarr**: An indexer manager/proxy for Sonarr, Radarr, and other applications.
- **Overseerr**: A request management and media discovery tool for your media server.
- **Homepage**: A simple, standalone homepage for monitoring and managing your media server.

## Getting Started

To get started with setting up your media server, follow these steps:

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/whipp-media-server.git
    cd whipp-media-server
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
    - Overseerr: `http://localhost:5055`
    - Homepage: `http://localhost:3000`

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

Enjoy your new media server setup!
