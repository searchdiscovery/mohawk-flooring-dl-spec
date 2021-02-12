## Internal Campaigns Displayed

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Internal Campaigns Displayed",
  "internalCampaign": {
    "campaignList": [
      {
        "internalCampaignID": "<internalCampaignID>",
        "internalCampaignCreative": "<internalCampaignCreative>",
        "internalCampaignName": "<internalCampaignName>"
      }
    ]
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|internalCampaignCreative|string|Describes the creative treatment for an internal campaign|Girl with bike, Mountain Top, River Cruise Danube|||||||
|internalCampaignID|string|Unique Identifier of an internal campaign|2345, 56789, 9876|||||||
|internalCampaignName|string|The name of the promotion.|Trek bikes for kids, REI Spring Sale 2019, Viking Cruise Fall Specials|||||||