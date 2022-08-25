# Interactive Milestone Reached

These HTML attributes should be added to items that are a part of interactive pages, rather than static pages, to track the milestone reached for user engagement.

## Generated Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Interactive Milestone Reached",
  "linkInfo": {
    "milestone": "<milestone>",
  }
});
```

### Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|milestone|string|Percent scrolled or specific milestone (title of a section of the page) reached from an interactive page|25%, 50%, 75%, 100%, etc. |
