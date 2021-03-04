## Order Placed

Set when a visitor completes their order for product samples. Note that the "productID" here is the production collection name as this is consistent throughout a visitors interactions with products from PLP > PDP > Sample Purchases.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Order Placed",
  "transaction": {
    "total": {
      "currency": "<currency>"
    },
    "item": [
      {
        "productInfo": {
          "productID": "<productID>",
          "brand": "<brand>",
          "name": "<name>",
          "sku": "<sku>",
          "isSample": "<isSample>",
          "productLine": "<productLine>",
          "trademarkedTechnology": "<trademarkedTechnology>",
          "color": "<color>"
        },
        "price": {
          "sellingPrice": "<sellingPrice>",
          "priceTier": "<priceTier>"
        },
        "quantity": "<quantity>",
        "shippingAddress": {
          "postalCode": "<postalCode>",
          "stateProvince": "<stateProvince>",
          "country": "<country>"
        }
      }
    ],
    "purchaseID": "<purchaseID>",
    "transactionID": "<transactionID>",
    "payment": [
      {
        "paymentMethod": "<paymentMethod>"
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|country|string|Indicates the country of the address of the shipment. ISO 3166 (alpha-2) Uppercase.|US, CA, FR, UK|^[A-Z]{2}$||||||
|currency|string|Currency of the transaction. ISO 4217 (3 character alpha), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|isSample|string|True/False flag to indicate if the product is a sample.|true, false|||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|paymentMethod|string|Describes the method of payment for a transaction. |Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|postalCode|string|The mailing zip or postal code associated with the address of the shipment. |53533, 30381, M1R 0E9, M3C 0C1|||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|purchaseID|string|Unique identifier of the purchase. Max Length 20. Used as Unique ID of the purchase or deduplication.|ABC-132456789, DEF-132456789, 0987654567|^[a-zA-Z0-9]{6,20}$|6|20||||
|quantity|integer|Integer number of products being acted upon (added to a cart, removed from wishlist, purchased, reserved)|1, 2, 3, 4, 5||||1|||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|stateProvince|string|The mailing state or province associated with address of the shipment. |WI, GA, NB, ON|||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||
|transactionID|string|Unique identifier of the transaction. Max Length 100. Used as a key for upload of post transaction data. |123e4567-e89b-12d3-a456-426614174000|^[a-zA-Z0-9]{6,100}$|6|100||||