## Listing Filter Added

After an onsite search for a product or a retailer is made and those results are then filtered or refined, this event will be set.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Listing Filter Added",
  "listingRefined": {
    "listingType": "<listingType>",
    "filterList": "<filterList>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|filterList|string|A twice delimited string of filterType and filterValue pairs.  Use ~ between type and value.  Use | between pairs|sort~price ascending|color~green|size~medium|||||||
|listingType|string|The type of listings shown|Product, Location, Event, Room, Content|||||||