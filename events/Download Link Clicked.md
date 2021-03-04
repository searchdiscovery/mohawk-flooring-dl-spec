## Download Link Clicked

Set on the click of any link that contains a document that can be downloaded (PDF, CSV, XLS, etc.). This will include product warrenty information, etc.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Download Link Clicked",
  "linkInfo": {
    "linkId": "<linkId>",
    "fileName": "<fileName>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|fileName|string|Indicates the filename for download link tracking.|Year End 2012.pdf, Operating Instructions.doc`|||||||
|linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||