## User Registered

Set upon the successfull creation of a new account by a visitor. This could happen at the top of the site or as a visitor moves through the order sample process.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Registered",
  "user": {
    "custKey": "<custKey>",
    "loginStatus": "<loginStatus>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||
|loginStatus|string|Describes the login state of the user|logged in, logged out, guest|||||||