# Using the Docsify service

## Prerequisites

### Docker Compose
```bash
sudo apt install docker-compose
```

## Installing the service

1. Copy the `docs.service` unit file into `/etc/systemd/system/docs.service`, editing as necessary for your repo.
   
2. Enable the service:
   ```bash
   sudo systemctl enable docs
   ```
3. Start the service:
   ```bash
   sudo systemctl start docs
   ```
   > :point_right: Note: The first start may take a while as the container image is built.

4. Add an HTTPS access method in UDF, pointing to port 3000.