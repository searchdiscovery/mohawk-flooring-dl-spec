## Location Detected

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Location Detected",
  "location": {
    "locationDeterminationMethod": "<locationDeterminationMethod>"
  },
  "locationList": [
    {
      "locationName": "<locationName>"
    }
  ]
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|locationDeterminationMethod|string|Describes how a location selection was determined.  Was it automatic or customer choice.|Automatic - IP based, Automatic - Device Based, Customer Selected|||||||
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||