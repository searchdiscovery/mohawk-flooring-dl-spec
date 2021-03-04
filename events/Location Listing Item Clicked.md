## Location Listing Item Clicked

Set when a visitor clickes either the "Make This My Retailer" option as a part of a dealer listing or if they click through to the dealer's detail page.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Location Listing Item Clicked",
  "listingItemClicked": {
    "listing": [
      {
        "itemPosition": "<itemPosition>",
        "location": {
          "locationType": "<locationType>",
          "locationId": "<locationId>",
          "locationName": "<locationName>"
        }
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||
|locationType|string|The type of the location|Retail Store, Lodging, ATM, Banking Branch|||||||