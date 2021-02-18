## Product Interaction Occurred

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Interaction Occurred",
  "product": [
    {
      "productInfo": {
        "productID": "<productID>",
        "productVisualization": "<productVisualization>",
        "productLine": "<productLine>",
        "brand": "<brand>",
        "trademarkedTechnology": "<trademarkedTechnology>",
        "name": "<name>",
        "sku": "<sku>",
        "color": "<color>"
      },
      "price": {
        "priceTier": "<priceTier>"
      }
    }
  ],
  "productInteraction": {
    "interactionDetail": "<interactionDetail>",
    "interactionType": "<interactionType>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|interactionDetail|string|Prodives details specific to the product Interaction type|Added to Favorites, Removed from Favorites, Front View, Side View|||||||
|interactionType|string|Describes the type of product interaction that occurred|Favorites Clicked, Thumbnail Image Clicked, Product Line Selected, Reviews Expanded|||||||
|name|string|||||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|productVisualization|string|Describes the visualization in which the product is presented. |Kitchen, Great Room, Bathroom, Bedroom, Custom|||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||