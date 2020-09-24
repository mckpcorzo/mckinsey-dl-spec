# Social Content Shared

Fire whenever a social share link is clicked, but do not fire on static link to a social network. Prioritize this last as it may change.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Social Content Shared",
  "social": {
    "socialNetwork": "<socialNetwork>",
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|socialNetwork|string|Describes the social network being acted upon (liked, followed, shared).|facebook, linkedin, instagram, twitter|