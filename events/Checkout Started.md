## Checkout Started

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Checkout Started",
  "product": [
    {
      "productInfo": {
        "productID": "<productID>",
        "name": "<name>",
        "sku": "<sku>"
      }
    }
  ],
  "cart": {
    "item": [
      {
        "productInfo": {
          "articleNumber": "<articleNumber>",
          "name": "<name>"
        }
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|articleNumber|string|||||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||