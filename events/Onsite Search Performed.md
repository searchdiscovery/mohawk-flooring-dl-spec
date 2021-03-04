## Onsite Search Performed

Set when a visitor first completes an onsite search for:
 - Products
 - Dealers

Note: Later filtering of search results is NOT a new instance of this event. This is only set at the initiation of a new search (i.e. from the site's header or retailer search function).

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Performed",
  "onsiteSearch": {
    "keyword": {
      "searchType": "<searchType>"
    }
  },
  "keywordSearch": {
    "fakeProductCollection": [
      {
        "fakeProductId": "<fakeProductId>"
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|fakeProductId|string|Helper node used by AA Product String Builder to set product to location. Set this field with a call to _satellite.getVar("fakeSearchProductId").  With updates to the AA PS extension, this will soon go away.|_satellite.getVar("fakeSearchProductId")|||||||
|searchType|string|Describes the domain of the search. |products, properties, articles, authors, coupons, publications|||||||