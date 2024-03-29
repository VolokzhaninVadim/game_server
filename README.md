# My game server
![](https://avatars.githubusercontent.com/u/115333610?s=200&v=4)

## Make directories
```sh
sudo mkdir -p game_server
sudo chown -R $(id -u):$(id -g) game_server
sudo mkdir -p game_server/{home,.X11-unix,pulse}
sudo chown -R $(id -u):$(id -g) game_server
sudo mkdir /mnt/media/games
sudo chmod -R 775 /mnt/media/games
sudo chown -R $(id -u):$(id -g) /mnt/media/games
touch game_server/docker-compose.yml
```

## Check NVIDIA
```
docker exec -it steam-headless-steam-headless-1 nvidia-smi
```

## Open server on browser
`http://ip_server:8083/`

## On client (Arch)
```
sudo pacman -S steam
flatpak install steamlink
```

[docker-steam-headless](https://github.com/Steam-Headless/docker-steam-headless?ysclid=lshi7ff4iv14641784)
