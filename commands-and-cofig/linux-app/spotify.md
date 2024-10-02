# Spotify specific configs and fixes on Linux

## HiDPI Scaling with Spotify and Flatpak.


Install spotify via flatpak using the instructions on flathub.

To force Spotify to scale properly, we can use the `--force-device-scale-factor=`` command line option (where X is the scaling factor).

E.g. X = 1.6 works pretty well.

To test, you can run


`flatpak run com.spotify.Client --force-device-scale-factor=1.6`

in your terminal.


In order to make this a permanent change, you can edit the desktop file (the one you have in your start menu or panel).


Navigate to the Flatpak shortcut directory:
`~/.local/share/applications/`
`

Edit the com.spotify.Client.desktop file as root with your favorite text editor.

`sudo nano com.spotify.Client.desktop`


Append the aforementioned command line argument to the end of the line starting with 'Exec'
`--force-device-scale-factor=1.6`


You can edit the "main" file for Spotify too, but that'll just be overwritten whenever Spotify updates.
Location for the "main" file: `/var/lib/flatpak/exports/share/applications/`
`


The effects should be seend immediately next time you launch Spotify.


Credits to https://justincaustin.com/blog/spotify-flatpak-hidpi-scaling
