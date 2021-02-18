## Product Added to Cart

Set when a visitor adds product samples to their cart. Note that the "productID" here is the production collection name as this is consistent throughout a visitors interactions with products from PLP > PDP > Sample Purchases.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Added to Cart",
  "product": [
    {
      "productInfo": {
        "productID": "<productID>",
        "brand": "<brand>",
        "isSample": "<isSample>",
        "name": "<name>",
        "sku": "<sku>",
        "productLine": "<productLine>",
        "trademarkedTechnology": "<trademarkedTechnology>",
        "color": "<color>"
      },
      "price": {
        "priceTier": "<priceTier>"
      }
    }
  ],
  "cart": {
    "additionContext": "<additionContext>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|additionContext|string|Conveys the context of a cart addition. |PLP, PDP, Wishlist, Registry|||||||
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|isSample|string|True/False flag to indicate if the product is a sample.|true, false|||||||
|multiAdditions|boolean|Flag indicating whether multilple products where added to carts, wishlists, registries, etc.|true, false|||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||
