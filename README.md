# Zoom-L-12-pulse
A pulse audio configuration for the Zoom L-12 (L12) Mixer to enable input/output separation

Tested on Manjaro KDE

## Install
1. Copy the .config folder to your home directory or more specifically the `default.pa`-file to `~/.config/pulse/default.pa` 
2. Restart Pulseaudio: `systemctl restart --user pulseaudio`

## Info
Use at own risk

- The device will be in the settings even if it's not connected
  - I first hoped to be able to make it only apply when the device is connected but couldn't quite get it to work as desired.
    So I just decided to let it be as it was good enough for my desktop setup
- As the Config is statically loaded it can be that it breaks especially after standby or when replugged.
  - Typically restarting pulseaudio is enough to make it work again


## Contribution is very welcome :)
If someone knows/finds a better way to solve this, I'd be very happy to see a PR. :)
