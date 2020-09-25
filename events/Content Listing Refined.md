# Content Listing Refined

Fire whenever a user clicks on a search feature that refines or otherwise modifies the search results.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Listing Refined",
  "listingRefined": {
    "searchType": "<searchType>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|searchType|string|Describes the type of search performed.|article, content, job, people, etc.|