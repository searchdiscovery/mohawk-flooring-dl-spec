## Video Started

Seet when a visitor starts viewing a video.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Video Started",
  "video": {
    "videoName": "<videoName>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|videoName|string|Video Name|Twitch_FPS, Age of Empires, Halo|||||||
