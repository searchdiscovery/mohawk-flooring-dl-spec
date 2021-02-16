## User Signed In

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Signed In",
  "user": {
    "custKey": "<custKey>",
    "loginStatus": "<loginStatus>",
    "userType": "<userType>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||
|loginStatus|string|Describes the login state of the user|logged in, logged out, guest|||||||
|userType|string|Describes the type of the user.  Often used to differentiate customers from employees or associates. |employee, guest, agent, customer|||||||