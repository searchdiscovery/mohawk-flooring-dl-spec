## Quiz Step Completed

Set when a visitor completes or answers any part of the flooring quiz.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Quiz Step Completed",
  "quiz": {
    "quizStepResponse": "<quizStepResponse>",
    "quizStep": "<quizStep>",
    "quizStepNumber": "<quizStepNumber>",
    "quizName": "<quizName>"
  }
});
```

|Field|Type|Description|Examples|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|quizName|string|The name of the quiz being tracked.  Should be the same for all steps within the quiz|Floor Chooser, Swim Finder, Movie Decider, My Next Book|||||||
|quizStep|string|Describes the step within a quiz. Should depict the question being asked.|Indoor / Outdoor, Durability, Mood|||||||
|quizStepNumber|integer|Indicates the step number within a multi-step quiz. |1, 2, 3, 4||||1|||
|quizStepResponse|string|Describes the reponse to a quiz step upon step completion|Hardwood, High Traffic, Happy, Fiction|||||||