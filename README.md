# riptag
Simple and effortless CD audio ripping, recognizing and tagging

# How it works?
`riptag` is a simple bash script that utilizes `cdparanoia` to rip individual audio tracks from CD into wave files, `ffmpeg` to covert wave files into format supported by it (like flac or mp3) and `acoustid` API to try and recognize ripped audio tracks. At the end, a series of simple shell commands is used to name and tag ripped audio tracks. Tagging tracks only works for a limited set of formats.

# How to use riptag?
If you want to rip a CD and convert it into mp3 simply run:
```bash
$ riptag --output-format mp3
```
By default `riptag` will automatically try and recognize ripped tracks, and if it succedes, it will name and tag every track, so that they are ready to use on the device of your choice. This is especially convinient if you import your music to a mp3 player or a cellphone.

# Does tagging and recognition works for every format?
Regognition and tagging work for most of the popular formats that support it. Some formats will only allow to recognize and name track files, but not tag them.

# Can I just use it for ripping?
Yes. Simply use --no-recognition and/or --no-tag switches. For full list of available options and switches issue `riptag --help` or `riptag -h`.
