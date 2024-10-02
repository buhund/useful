# Macos 

## Mac startup chime:

### Disable startup chime
`sudo nvram SystemAudioVolume=%80`

### Enable startup chime:
`sudo nvram -d SystemAudioVolume`

### Alternative disables:

`sudo nvram SystemAudioVolume=%01`

`sudo nvram SystemAudioVolume=%00`

`sudo nvram SystemAudioVolume=" "`

