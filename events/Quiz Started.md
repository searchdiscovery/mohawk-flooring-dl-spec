## Quiz Started

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Quiz Started",
  "quiz": {
    "quizName": "<quizName>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|quizName|string|The name of the quiz being tracked.  Should be the same for all steps within the quiz|Floor Chooser, Swim Finder, Movie Decider, My Next Book|||||||