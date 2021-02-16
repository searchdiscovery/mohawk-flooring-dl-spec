## Listing Filter Removed

While viewing a set of onsite search results for products or retailers, if a filter or refinement is removed, this event will be set.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Listing Filter Removed",
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
