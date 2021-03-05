## Basic Commands

- Audio/Video Information

```
ffmpeg -i video.mp4
```

- Convert files

```
ffmpeg -i video.mp4 video.mkv
```

- Convert movie file to mp3

```
ffmpeg -i sample.avi -q:a 0 -map a sample.mp3
```

```
ffmpeg -i sample.avi -ss 00:01:00 -t 00:10:00.0 -q:a 0 -map a sample.mp3
```

- Change video resolution

```
ffmpeg -i input.mp4 -filter:v scale=1280:720 -c:a copy output.mp4
```

- Cutting Videos

```
fmpeg -i movie.mp4 -ss 00:00:03 -t 00:00:08 -async 1 -c copy cut.mp4
```

## Reference

- https://ostechnix.com/20-ffmpeg-commands-beginners/
- https://stackoverflow.com/questions/18444194/cutting-the-videos-based-on-start-and-end-time-using-ffmpeg
