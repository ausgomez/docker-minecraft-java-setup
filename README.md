# Docker Setup for Minecraft

## Requirements

1. Linux Server
2. Docker Installed on Server
3. Docker Compose Installed
4. Minecraft Java edition

## How to Install it using Digital Ocean

1. Create a Digital Ocean Account for free using this link to get $100 credit!!
   - https://m.do.co/c/e74eb9516ce5

2. Create an Ubuntu server with minimum of 4GB of RAM

3. Connect to the server using ssh
   - Example:
     - `$ ssh root@your-server-ip-address`
4. Install `Docker` using the convenience script:
   - Follow these steps:
     https://docs.docker.com/engine/install/ubuntu/#install-using-the-convenience-script

5. Install `Docker Compose`
   - Follow these steps: https://docs.docker.com/compose/install/

6. Git clone this same repo on your server or just copy the `docker-compose.yml`
   file

7. Run the docker compose file:
   - `$ docker-compose up -d`

8. Open Minecraft and direct connect to the server

## Allow Cracked Accounts to play on your server (Optional)

If you run this server as it comes, you can only play it if you have bought
Minecraft, but you could also play it for free using
[TLauncher](https://tlauncher.org/en/)

1. Navigate to `/minecraft-data` folder
2. Edit the `server.propeties` file and change:
   - `online-mode=true` to `online-mode=false`
3. Restart the server:
   - `$ docker-compose restart`
