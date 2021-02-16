## Social Brand Followed

Set when a visitor clicks one of the social account links that are present in the footer (or other locations) of the site.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Social Brand Followed",
  "social": {
    "socialNetwork": "<socialNetwork>",
    "accountFollowed": "<accountFollowed>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|accountFollowed|string|Describes the specific social network account (of your brand) that is being followed.|sditech@twitter.com, searchdiscovery@linkedIn.com|||||||
|socialNetwork|string|Describes the social network being acted upon (liked, followed, shared). |facebook, linkedIn, instrgram, twitter|||||||
