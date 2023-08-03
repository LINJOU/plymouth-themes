# plymouth-themes

some plymouth themes

+ fedora-plymouth
    fork: https://www.gnome-look.org/p/2035462
+ vinyl
    fork: https://www.gnome-look.org/p/1000036

## Installation

### install plymouth

```shell
sudo dnf install -y plymouth
```

### update grub2

+ editor `/etc/default/grub`
  `GRUB_CMDLINE_LINUX_DEFAULT=splash`
+ update grub2
  ```shell
  grub2-mkconfig -o /boot/grub2/grub.cfg
  ```

### add plymouth themes

```shell
git clone https://github.com/LINJOU/plymouth-themes.git
cd plymouth-themes
sudo cp themes /usr/share/plymouth/themes
```

### check out plymouth themes

```shell
sudo plymouth-set-default-theme -l
```

### install plymouth themes

```shell
sudo plymouth-set-default-theme -R yourtheme
```
