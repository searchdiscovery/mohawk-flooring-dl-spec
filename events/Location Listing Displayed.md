## Location Listing Displayed

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Location Listing Displayed",
  "listingDisplayed": {
    "listing": [
      {
        "location": {
          "fakeProductId": "<fakeProductId>",
          "locationId": "<locationId>",
          "locationName": "<locationName>",
          "locationType": "<locationType>"
        },
        "isDisplayed": "<isDisplayed>",
        "itemPosition": "<itemPosition>"
      }
    ],
    "resultsCount": "<resultsCount>",
    "displayCount": "<displayCount>",
    "listingType": "<listingType>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|displayCount|integer|The total number of items displayed out of all returned items. (Integer)|10, 20, 30, 40||||0|||
|fakeProductId|string|Helper node used by AA Product String Builder to set product to location. This field gets a static value of "location".  With updates to the AA PS extension, this will soon go away.|location|location||||||
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|locationName|string|The friendly name of the location.|Deerefiled Outlet, Old Orchard, Manhatten Midtown|||||||
|locationType|string|The type of the location|Retail Store, Lodging, ATM, Banking Branch|||||||
|resultsCount|integer|The total number of items returned that matched the search criteria. (Integer)|1, 21, 111, 166||||0|||