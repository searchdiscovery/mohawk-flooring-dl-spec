## Page Load Completed

After all page-level events have occured this event will fire. This is the indicator that no other events will be dispatched at this point, without additional visitor interactions with the site. This is only set after the concept of a page load.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Completed"
});
```