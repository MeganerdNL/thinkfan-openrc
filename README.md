# thinkfan-openrc
OpenRC init file for [thinkfan](https://github.com/vmatare/thinkfan).

## Prerequisites / Dependencies:
- A ThinkPad running linux with OpenRC as init system.
- Fancontrol enabled in *thinkpad_acpi* module. This is autmatically enabled when thinkfan is installed.
- [thinkfan](https://github.com/vmatare/thinkfan) installed - You can install it [from the AUR](https://aur.archlinux.org/packages/thinkfan) if you use (an) Arch (based distribution).

## Installation:
#### From [AUR](https://aur.archlinux.org/packages/thinkfan-openrc)
- `yay -S thinkfan-openrc` - or with your own favorite AUR helper.
- Add the service to default runlevel with `rc-update add thinkfan`
- Start the service with `rc-service thinfan start`
#### Manual
- Place the file *thinkfan* from this repository in */etc/init.d* and make it executeable: `chmod +x thinkfan`.
- Create a file */etc/thinkfan.conf*. Example is in: */usr/share/doc/thinkfan/examples/thinkfan.yaml*
- Add the service to default runlevel with `rc-update add thinkfan`
- Start the service with `rc-service thinkfan start`

## Further documentation:
See [thinkfan](https://github.com/vmatare/thinkfan) and the [Arch Wiki](https://wiki.archlinux.org/title/Fan_speed_control#ThinkPad_laptops).
