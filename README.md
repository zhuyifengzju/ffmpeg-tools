# ffmpeg-tools
A collection of commands to use ffmpeg to do simple video clips



### MTS file to mp4
```
ffmpeg -i NAME.MTS -c:v copy NAME.mp4
```


### Clip a video
```
 ffmpeg -i NAME.mp4 -ss 00:00:10 -t 00:00:40 -c copy -an NAME_part.mp4
```

### Speed up a video
```
 ffmpeg -i NAME.mp4 -filter:v "setpts=0.1*PTS" NAME_fast.mp4
```
