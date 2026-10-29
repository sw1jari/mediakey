# mediakey

Handler for the keyboard's play/pause, next and previous keys.

If the mpv started by [music-menu](https://github.com/sw1jari/music-menu) is running, it controls that. Otherwise it falls back to `playerctl`, so the keys still work with other players like Firefox or Spotify.

## Requirements
socat, playerctl

## Install
```sh
cp mediakey ~/.local/bin/
```

## Usage
```sh
mediakey play-pause
mediakey next
mediakey previous
```

Bind it in your hotkey daemon, like in sxhkd:
```
XF86AudioPlay
    mediakey play-pause
XF86AudioNext
    mediakey next
XF86AudioPrev
    mediakey previous
```
