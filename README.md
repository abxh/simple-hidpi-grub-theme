# simple-hidpi-grub-theme
a minimalistic grub theme made for hidpi screens.

```
git clone https://github.com/abxh/simple-hidpi-grub-theme
mkdir -p /boot/grub/themes
cp -r simple-hidpi-grub-theme /boot/grub/themes/
echo 'GRUB_THEME="/boot/grub/themes/simple-hidpi-grub-theme/theme.txt"' >> /etc/default/grub
```

replace the `font.pf2` to the desired font for one's dpi.
```
# for terminus-font in arch
cp /usr/share/grub/ter-u28b.pf2 /boot/grub/themes/simple-hidpi-grub-theme/font.pf2
```
