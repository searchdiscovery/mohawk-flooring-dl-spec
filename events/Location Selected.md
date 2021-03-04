## Location Selected

Set when a location is selected by (Make This My Retailer) or assigned (Geo IP Lookup) to the visitor. locationDeterminationMethod indicates if a visitor is currently browsing with a selected location or the one that was assigned by Geo IP detection.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Location Selected",
  "locationList": [
    {
      "locationName": "<locationName>",
      "locationId": "<locationId>"
    }
  ]
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||