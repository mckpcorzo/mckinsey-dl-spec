# Content Listing Item Clicked

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Social Content Shared",
  "listingItemClicked": {
    "itemPosition": "<itemPosition>",
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5|