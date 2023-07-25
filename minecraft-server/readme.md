# Minecraft Server

```
$ sudo docker run -d -it -p 25565:25565 -e EULA=TRUE -e INIT_MEMORY=1G MAX_MEMORY=2G -v /home/leo/minecraft-server-data:/data itzg/minecraft-server
```