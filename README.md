# hushmeet

Tool for me to juggle several google meets and a severe tab hoarding issue.

Put it in `$PATH` and make cool `aliases` or hotkeys. Maybe that `flic-button` you have in a drawer.

## Prerequisites
OSX, chrome and `Allow JavaScript from Apple Events` turned on in chrome

## Usage

```
./hushmeet
Usage: cmds... [id]
cmds:
    status - finds and logs meets
    goto - navigates to meet [id] or first if not specified. breaks mute of "all".
    mm - mutes mic for meet [id] or all if not specified
    mc - mutes camera for meet [id] or all if not specified
    toggle - toggles audio for meet [id] or all if not specified
    
    ma - mutes out audio for meet [id] or all if not specified
    uma - unmutes out audio for meet [id] or all if not specified
cmds apart from status can be combined. eg. "goto mm" navigates and mutes the first meet found
```

show some status about meets found among chrome windows and tabs.
```
./hushmeet status
NAME                    MIC MUTED       CAMERA MUTED	URL
Meet – Stand up         false           false	        https://meet.google.com/abc-asdf-ghj?authuser=1
Meet – xyz-asdf-pjh     false           false	        https://meet.google.com/xyz-asdf-pjh?authuser=1
```

navigate to first found meet
```
./hushmeet goto
```

navigate to meet containing `pjh` in url
```
./hushmeet goto pjh
```

navigate to first meet and mute your mic
```
./hushmeet goto mm
```

mute mic and camera on meet containing `pjh` in url
```
./hushmeet mm mc pjh
```

mute mic on all meets found
```
./hushmeet mm
```
