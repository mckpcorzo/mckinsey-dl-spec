# Generic Event Occurred

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Generic Event Occurred",
  "genericEvent": {
    "action": "<action>",
    "category": "<category>",
    "label": "<label>",
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|action|Used to capture the associated category of the generic interaction event|footnote links,  related article link, podcast start, etc.|
|category|Used to capture the associated action of the generic interaction event|click, play, impression, start, etc.|
|label|Used to capture the associated label of the generic interaction event|footnote #, related article name, podcast name, etc.|