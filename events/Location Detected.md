## Location Detected

As a visitor moves through the site, information about their currently selected location will be stored here. locationDeterminationMethod indicates if a visitor is currently browsing with a selected location or the one that was assigned by Geo IP detection.

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
          "locationId": "<locationId>",
          "locationName": "<locationName>",
          "locationType": "<locationType>"
    }
  ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|locationDeterminationMethod|string|Describes how a location selection was determined.  Was it automatic or customer choice.|Automatic - IP based, Automatic - Device Based, Customer Selected|||||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||
|locationType|string|Concatenation of channel and edge tier|speciality~tier value||||||
