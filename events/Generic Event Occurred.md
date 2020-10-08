# Generic Event Occurred

Fire whenever a generic event with no specific built-in or custom dimensions or metrics occurs. For click events, you can leverage the data attribute spec instead of pushing the DL events manually.

## Data Attributes HTML Code

```html
  <a href="<linkDestination>"
    data-layer-event="Generic Event Occurred"
    data-layer-action="click"
    data-layer-generic-action="<action>"
    data-layer-generic-category="<category>"
    data-layer-generic-label="<linkText?>"
  >
```

Items with a ? are optional

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Generic Event Occurred",
  "genericEvent": {
    "action": "<action>",
    "category": "<category>",
    "label": "<label>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|action|string|Used to capture the associated action of the generic interaction event|click, play, impression, start, etc.|
|category|string|Used to capture the associated category of the generic interaction event|footnote links,  related article link, podcast start, etc.|
|label|string|Used to capture the associated label of the generic interaction event|footnote #, related article name, podcast name, etc.|