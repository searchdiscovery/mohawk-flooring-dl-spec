## Exit Link Clicked

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Exit Link Clicked",
  "linkInfo": {
    "linkId": "<linkId>",
    "linkTarget": "<linkTarget>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|linkId|string|Identifier of the link clicked|act now, cancel, ok, 3456, 8765|||||||
|linkTarget|string|HREF of the link.  Primarily useful for exit link tracking. |https://www.usda.gov. https://msnbc.com|||||||