# SteamWaydroidLauncher

Launch Waydroid Android apps in Steam with controller support.

Based on scripts from the [Bazzite project](https://github.com/ublue-os/bazzite).

## Features

- Caged Waydroid environment using `cage`
- Add Android apps to Steam
- Automatic controller configuration
- Resolution detection
- Desktop menu integration

## Prerequisites

Initialize Waydroid:
```bash
sudo waydroid init
```

See [Waydroid docs](https://docs.waydro.id/) for setup.

## Installation

### Arch Linux (AUR)
```bash
paru -S steamwaydroidlauncher-git
```

### Manual Installation
```bash
# Install to system directories
sudo cp bin/* /usr/bin/
sudo cp lib/* /usr/lib/swl/
sudo cp desktop/* /usr/share/applications/
sudo cp polkit-1/actions/* /usr/share/polkit-1/actions/
sudo cp polkit-1/rules.d/* /usr/share/polkit-1/rules.d/
sudo cp share/* /usr/share/swl/
```

## Usage

### Launch Waydroid
```bash
# Full Waydroid interface
swl-launch

# Specific Android app
swl-launch app launch com.example.app
```

### Add Apps to Steam
```bash
swl-add-waydroid-app
```

### Desktop Applications
Application menu → "SWL" category:
- SWL: Launch Waydroid
- SWL: Add Waydroid App to Steam
- SWL: Stop Waydroid

## Dependencies

- `bash`, `waydroid`, `cage`, `wlr-randr`, `xorg-xrandr`, `kdialog`, `polkit`

## Credits

Scripts from [Bazzite](https://github.com/ublue-os/bazzite).

## License

GPL-3.0
