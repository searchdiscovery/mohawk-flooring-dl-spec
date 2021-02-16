## Navigation Link Clicked

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Navigation Link Clicked",
  "linkInfo": {
    "linkId": "<linkId>",
    "linkRegion": "<linkRegion>",
    "linkContainer": "<linkContainer>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkContainer|string|Indicates the container for a clicked link within the hierarchy [Site > Page > Region > Container > linkID]|Best Friends - Best Jeans, Puppy Love, Sail Away, Mens, Kids, Kids : Tops|||||||
|linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkRegion|string|Indicates the region on page for a clicked link within the hierarchy [Site > Page > Region > Container > linkID]|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||