<div align="center">
    <img src="/img/README-decorator.png" width=300/><br/>
    <a href="https://github.com/AllJavi/tartarus-grub/stargazers">
        <img src="https://img.shields.io/github/stars/AllJavi/tartarus-grub?color=a9b665&style=for-the-badge&logo=starship">
    </a>
    <a href="https://github.com/AllJavi/tartarus-grub/issues">
        <img src="https://img.shields.io/github/issues/AllJavi/tartarus-grub?color=ea6962&style=for-the-badge&logo=codecov">
    </a>
    <a href="https://github.com/AllJavi/tartarus-grub/network/members">
        <img src="https://img.shields.io/github/forks/AllJavi/tartarus-grub?color=7daea3&style=for-the-badge&logo=jfrog-bintray">
    </a>
    <a href="https://github.com/AllJavi/tartarus-grub/blob/main/LICENSE">
        <img src="https://img.shields.io/badge/license-MIT-orange.svg?color=d4be98&style=for-the-badge&logo=archlinux">
    </a>
</div>

## Preview
![preview](/img/low-res.png)

## Compatibility
This should work on any Linux distribution that uses GRUB, but I have only tested it on EndeavourOS and Kali

## Install
```bash
git clone https://github.com/AllJavi/tartarus-grub.git
cd tartarus-grub
sudo cp tartarus -r /usr/share/grub/themes/
sudo vim /etc/default/grub
```
Change `#GRUB_THEME=` to
`GRUB_THEME="/usr/share/grub/themes/tartarus/theme.txt"`
```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
If all works correctly you should get this line in the out put:
```bash
Found theme: /usr/share/grub/themes/tartarus/theme.txt
```

#### NOTE: For Fedora 37
When editing the file `/etc/default/grub`, you also have to comment the line `'GRUB_TERMINAL_OUTPUT="console"`

## Credit
- [Cute Ghost profile](https://www.flaticon.com/free-icon/ghost_1150381?term=ghost&page=1&position=52&page=1&position=52&related_id=1150381&origin=style)
- [Dracula Grub](https://draculatheme.com/grub)
- [Tokyo Night Grub](https://github.com/mino29/tokyo-night-grub)

## License
[MIT License](./LICENSE)
