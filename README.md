# simple-hidpi-grub-theme
A system-boot-inspired grub theme made for a hidpi 1980x1080 screen.

Probably looks like how you expect of it. If you want a preview, then see [bad preview](https://github.com/abxh/simple-hidpi-grub-theme/blob/main/bad_preview.jpg).

## Install instructions
Clone this repository.
```
git clone --depth=1 --branch=main https://github.com/abxh/simple-hidpi-grub-theme
```

> The steps after this should be done as the superuser or through tools like `sudo`.

Copy the theme to `/boot/grub/themes`. 
```
mkdir -p /boot/grub/themes
cp -r simple-hidpi-grub-theme/src /boot/grub/themes/simple-hidpi-grub-theme
```

Set the theme by changing the `GRUB_THEME` variable in `/etc/default/grub`.
```
# /etc/default/grub
GRUB_THEME="/boot/grub/themes/simple-hidpi-grub-theme/theme.txt"
```

Update the grub config.
```
grub-mkconfig -o /boot/grub/grub.cfg
```

## Optional
Replace the `font.pf2` to the desired font for one's dpi.
```
# for terminus-font in arch
cp /usr/share/grub/ter-u28b.pf2 /boot/grub/themes/simple-hidpi-grub-theme/font.pf2
```
