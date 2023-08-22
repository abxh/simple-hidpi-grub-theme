# simple-hidpi-grub-theme
a minimalistic grub theme made for hidpi screens.

```
git clone --depth=1 --branch=main https://github.com/abxh/simple-hidpi-grub-theme
rm -rf ./simple-hidpi-grub-theme/.git
su
mkdir -p /boot/grub/themes
cp simple-hidpi-grub-theme /boot/grub/themes/
echo "https://github.com/abxh/simple-hidpi-grub-theme
```

replace the `font.pf2` to the desired font for one's dpi.
```
# for terminus-font in arch
cp /usr/share/grub/ter-u28b.pf2 /boot/grub/themes/simple-hidpi-grub-theme/font.pf2
```
