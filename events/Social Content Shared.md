# Social Content Shared

Fire whenever a social share link is clicked, but do not fire on static link to a social network. Prioritize this last as it may change.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Social Content Shared",
  "social": {
    "socialNetwork": "<socialNetwork>",
    "thingShared": "<thingShared>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|socialNetwork|string|Describes the social network being acted upon (liked, followed, shared).|facebook, linkedIn, instrgram, twitter|
|thingShared|string|Specific description of the thing being shared to a social network.|product56769, article1343, Post2908|
