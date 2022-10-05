# gitea

A docker compose file for my gitea environment.

## Usage 

### Starting

```bash
cd ~/gitea            # change to the gitea directory
docker compose pull   # pulls the latest images
docker compose up -d  # starts containers 
```

Once up and running, using a web browser got to http://dockerhost:3000 and complete the installation.

### Stopping

```bash
docker compose down  # stops the container
```

### Updating

```bash
cd ~/gitea                      # change to the gitea directory
docker compose pull             # pulls the latest images
docker compose up -d --no-deps  # restarts the containers with the newer images
docker system prune -a          # deletes any unused images
```

### Uninstall

```bash
cd ~/gitea              # change to the gitea directory
docker compose down -v  # stops the containers and deletes the data volumes
docker system prune -a  # deletes any unused container images
```

## License

MIT

## Author Information

This project was created in 2022 by Graham Lillico.