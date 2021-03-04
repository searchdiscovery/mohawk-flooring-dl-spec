## Product Listing Item Clicked

Set whenever a visitor clicks through from a product detail listing for an item to its product detail page. This could be the "Shop" button, the product image, or any other item that sends the visitor to the subsequent product detail page. Note that the "productID" here is the production collection name as this is consistent throughout a visitors interactions with products from PLP > PDP > Sample Purchases.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Listing Item Clicked",
  "listingDisplayed": {
    "sortOrder": "<sortOrder>"
  },
  "listingItemClicked": {
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
        "itemPosition": "<itemPosition>",
        "price": {
          "currency": "<currency>",
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
|currency|string|Currency of the prices given. ISO 4217 (3 character alpha), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|sortOrder|string|Indicates the sort order.|high-low, low-high, nearest-farthest, a-z, newest-oldest|||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||