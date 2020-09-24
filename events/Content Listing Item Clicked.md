# Content Listing Item Clicked

Fire whenever a user clicks on a search result listing (job, employee profile, or content item, etc).

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Listing Item Clicked",
  "listingItemClicked": {
    "itemPosition": "<itemPosition>"
    "pageNumber": "<resultsPageNumber>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5|
|pageNumber|integer|The current pagination page number of the search result clicked.|1,2,3|
