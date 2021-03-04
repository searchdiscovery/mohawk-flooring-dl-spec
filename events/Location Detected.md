## Location Detected

As a visitor moves through the site, information about their currently selected location will be stored here. locationDeterminationMethod indicates if a visitor is currently browsing with a selected location or the one that was assigned by Geo IP detection.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Location Detected",
  "locationList": [
    {
      "locationName": "<locationName>"
    }
  ]
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||