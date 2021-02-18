## Internal Campaign Clicked

"When a content widget is clicked through (if its impression was previously measured) the click of that widget will result in this event being set. Note that "productID" here will be the descriptor or ID associated with the particular content widget.

- Campaign Creative: Will be populated with the name/descriptor of the content widget
- Campaign Position: Will be populated with the descriptor of the position of the content on the page"

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Internal Campaign Clicked",
  "internalCampaign": {
    "campaignList": [
      {
        "internalCampaignID": "<internalCampaignID>",
        "internalCampaignName": "<internalCampaignName>",
        "internalCampaignCreative": "<internalCampaignCreative>",
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
