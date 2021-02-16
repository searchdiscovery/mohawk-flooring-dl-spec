## Form Started

Set when a visitor starts a form (that is not Contact Us) by placing their cursor in a text field or otherwise first interacts with the form. This would include the Quote Request Form (and any others as applicable)

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Form Started",
  "form": {
    "formID": "<formID>",
    "formName": "<formName>",
    "formType": "<formType>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|formID|string|Unique identifier of a form. |F-0113, 2543, CU001, PI-0988|||||||
|formName|string|Plain text form name. Generally used if formID is not obtainable. |Payment Info, Mailing Address, Payment Address, Contact Us|||||||
|formType|string|Form type used for grouping of similar forms in reports.  |Quote|||||||
