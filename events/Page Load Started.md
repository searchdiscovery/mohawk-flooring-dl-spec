## Page Load Started

Set when a visitor moves to a new page.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
  "page": {
    "pageName": "<pageName>",
    "breadCrumbs": "<breadCrumbs>",
    "pageType": "<pageType>",
    "pageCategory": "<pageCategory>",
    "siteName": "<siteName>",
    "siteLanguage": "<siteLanguage>",
    "siteCountry": "<siteCountry>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|breadCrumbs|unknown|||||||||
|pageCategory|string|General category or Site Section of the page. Top level of page hierarchy.|Home, About Us, Shop, Account, Blog, Investors|||||||
|pageName|string|Describes the page and its content specifically. Here is recommendation. https://docs.google.com/presentation/d/1MBQb6cALPDzFiy2Vd-x8i_x9fA7NY3w3Pir8Ji1EofM/edit?usp=sharing |product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|pageType|string|Describes what purpose the page serves. Often aligns with the CMS template.|Home, Event Detail, Property Detail, Product Listing, Blog Post, Shopping Cart|||||||
|siteCountry|string|Indicates the primary country served by the site. ISO 3166 (alpha-2) Uppercase.|US, CA, FR, UK|^[A-Z]{2}$||||||
|siteLanguage|string|Language in which the site is presented ISO 639-1 code. |en-us, en-gb, ch-cn, fr-ca, fr-fr, da|^[a-z]{2}([-]{1}[a-z]{2}){0,1}$||||||
|siteName|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
