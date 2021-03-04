## Visualizer Viewed

Set when a visitor views the visualizer on a product detail page or via the "Discover" option from the main menu. The "product" array here will only be populated with the visualizer is frist viewed, within a product detail page.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Visualizer Viewed",
  "product": [
    {
      "productInfo": {
        "productID": "<productID>",
        "productVisualization": "<productVisualization>",
        "brand": "<brand>",
        "productLine": "<productLine>",
        "trademarkedTechnology": "<trademarkedTechnology>",
        "name": "<name>",
        "sku": "<sku>",
        "color": "<color>"
      },
      "price": {
        "priceTier": "<priceTier>",
        "priceType": "<priceType>"
      }
    }
  ]
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|name|string|||||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|priceType|string|Describes the type of price offered using commonly used terms. |1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|productVisualization|string|Describes the visualization in which the product is presented. |Kitchen, Great Room, Bathroom, Bedroom, Custom|||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||