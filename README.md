# Zoom-L-12-pulse
A pulse audio configuration for the Zoom L-12 (L12) Mixer to enable input/output separation on Linux.

**Use at own risk**

Tested on Manjaro KDE

## Install
1. Copy the .config folder to your home directory or more specifically the `default.pa`-file to `~/.config/pulse/default.pa`
2. Enable Class Compliant Mode (Switch on back of the L12)
3. Restart Pulseaudio: `systemctl restart --user pulseaudio`

## Info
The default.pa is a copy from `/etc/pulse/default.pa` that has been modified to use the L12. The base file will be ignored if pulse finds that a configuration in the home directory `~/.config/pulse/default.pa` is present.

- The device will be in the settings even if it's not connected
  - I first hoped to be able to make it only apply when the device is connected but couldn't quite get it to work as desired.
    So I just decided to let it be as it was good enough for my desktop setup
- As the Config is statically loaded it can be that it breaks especially after standby or when replugged.
  - Typically restarting pulseaudio is enough to make it work again


## Contribution is very welcome :)
If someone knows/finds a better way to solve this, I'd be very happy to see a PR. :)
