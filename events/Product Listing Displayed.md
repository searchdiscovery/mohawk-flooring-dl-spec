## Product Listing Displayed

Set on the view or product listing pages. Note that the "productID" here is the production collection name as this is consistent throughout a visitors interactions with products from PLP > PDP > Sample Purchases.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Listing Displayed",
  "listingDisplayed": {
    "filterListLength": "<filterListLength>",
    "filterList": "<filterList>",
    "sortDefault": "<sortDefault>",
    "listingType": "<listingType>",
    "resultsCount": "<resultsCount>",
    "listing": [
      {
        "productInfo": {
          "productID": "<productID>",
          "brand": "<brand>",
          "name": "<name>",
          "sku": "<sku>",
          "productLine": "<productLine>",
          "trademarkedTechnology": "<trademarkedTechnology>",
          "color": "<color>"
        },
        "isDisplayed": "<isDisplayed>",
        "itemPosition": "<itemPosition>",
        "price": {
          "priceTier": "<priceTier>"
        }
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|filterList|string|A twice delimited string of filterType and filterValue pairs.  Use ~ between type and value.  Use | between pairs|sort~price ascending|color~green|size~medium|||||||
|filterListLength|integer|The number of filterValue pairs in the filterList|0, 20, 12||||0|||
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|resultsCount|integer|The total number of items returned that matched the search criteria. (Integer)|1, 21, 111, 166||||0|||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|sortDefault|integer|The default sort value on listings|A to Z, Low to High, Newest to Oldest||||0|||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||