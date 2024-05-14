# Softwares

## Fcitx 5
[安装配置 Fcitx 5](https://muzing.top/posts/3fc249cf/)

```
sudo apt install fcitx5
sudo apt install fcitx5-chinese-addons
sudo apt install fcitx5-frontend-gtk4 fcitx5-frontend-gtk3 fcitx5-frontend-gtk2
sudo apt install fcitx5-frontend-qt5
```

## solaar
[Keyboard Logitech K780 supported on Mint 20.1 Cinnamon?](https://forums.linuxmint.com/viewtopic.php?t=346656)

```
sudo apt install solaar
```

## V2RayA
[新一代 Linux 客户端安装配置教程](https://yuqi.fun/posts/a53fea94.html)

```
wget -qO - https://apt.v2raya.org/key/public-key.asc | sudo tee /etc/apt/keyrings/v2raya.asc
echo "deb [signed-by=/etc/apt/keyrings/v2raya.asc] https://apt.v2raya.org/ v2raya main" | sudo tee /etc/apt/sources.list.d/v2raya.list
sudo apt update
sudo apt install v2raya v2ray

sudo systemctl start v2raya.service
sudo systemctl enable v2raya.service
```

软件配置链接：http://localhost:2017/
管理员帐号重置命令：`sudo v2raya --reset-password`

# Q & A

## sudo apt update
[How to fix "E: The list of sources could not be read" error?](https://stackoverflow.com/questions/42410134/how-to-fix-e-the-list-of-sources-could-not-be-read-could-not-be-read-error)

```
ls /etc/apt/sources.list.d/
sudo rm -r /etc/apt/sources.list.d/<list name>
```
