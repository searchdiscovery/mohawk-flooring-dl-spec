## Video Milestone Reached

Set when a visitor reaches the 25%, 50% and 75% milestone of a video.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Video Milestone Reached",
  "video": {
    "milestone": "<milestone>",
    "videoName": "<videoName>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|milestone|string|The milestone being tracked as an integer less than 100|25, 50, 77, 99|||||||
|videoName|string|Video Name|Twitch_FPS, Age of Empires, Halo|||||||