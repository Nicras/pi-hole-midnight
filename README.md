# pi-hole-plex

Custom plex theme CSS for pi-hole to replace skin-blue AdminLTE theme.

Created for use with [pi-hole](https://github.com/pi-hole/pi-hole).

[![Screenshot](https://github.com/Nicras/pi-hole-plex/blob/master/images/screenshot.jpg)](https://github.com/Nicras/pi-hole-plex/blob/master/images/screenshot.jpg)

---

## Install

Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/vendor/
sudo git clone https://github.com/nicras/pi-hole-plex.git
sudo rm -f skin-blue.min.css
sudo cp pi-hole-plex/skin-blue.min.css .
sudo cp pi-hole-plex/images/plex-bg.png /var/www/html/admin/img
sudo rm -rf pi-hole-plex
```

Don't forget the trailing " ." on the cp line (it means copy to current directory).

## Uninstall/Revert

Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/vendor/
sudo git reset --hard
```

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Credits

All credits for the initial work go to [Jacob bates](https://github.com/jacobbates/pi-hole-midnight).
