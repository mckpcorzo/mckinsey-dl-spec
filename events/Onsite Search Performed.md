# Onsite Search Performed

Fire whenever a user performs a search.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Onsite Search Performed",
  "listingRefined": {
    "searchType": "<searchType>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|searchType|string|Describes the type of search performed.|article, content, job, people, etc.|