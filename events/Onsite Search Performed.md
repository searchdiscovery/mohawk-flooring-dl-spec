## Onsite Search Performed

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Performed",
  "onsiteSearch": {
    "keyword": {
      "searchTerm": "<searchTerm>",
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
|searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion. |bluth, blue, red lobster|||||||
|searchType|string|Describes the domain of the search. |products, properties, articles, authors, coupons, publications|||||||