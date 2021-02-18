## Internal Campaigns Displayed

The site will have various content widgets where their impressions will need to be measured. When such content exists, this event will be set and popualted with an array of such content. Note that "productID" here will be the descriptor or ID associated with the particular content widget.

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
        "internalCampaignName": "<internalCampaignName>",
        "internalCampaignPosition": "<internalCampaignPosition>"
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
|internalCampaignPosition|integer|The position of a internal campaign offering within a list of internal campaigns|1, 5, 78, 3||||1|||
