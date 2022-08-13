# Thunderbird

## Update Thunderbird from tarball:

Extract archive

`cd thunderbird`

`sudo cp -r * /usr/lib/thunderbird`

## Hold Thunderbird package from PPA

Prevent apt from overwriting your manual updates

```
echo "Package: thunderbird
Pin: release release o=LP-PPA-mozillateam
Pin-Priority: -10" | sudo tee /etc/apt/preferences.d/manualThunderbird.pref
```



