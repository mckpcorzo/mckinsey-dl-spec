# Social Link Clicked

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Social Content Shared",
  "linkInfo": {
    "socialNetwork": "<socialNetwork>",
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|socialNetwork|string|Describes the social network being acted upon (liked, followed, shared).|facebook, linkedIn, instrgram, twitter|