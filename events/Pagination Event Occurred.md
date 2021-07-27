# Pagination Event Occurred

Fire when a user interacts with pagination controls or when results load automatically via scroll

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Pagination Event Occurred",
  "pagination": {
    "paginationContentType": "<paginationContentType>",
    "paginationPage": "<paginationPage>",
    "paginationType": "<paginationType>",
  }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|paginationContentType|string|The type of content represented by the |blog posts, jobs, global search results|
|paginationPage|integer|The page # of the results requested/loaded. Optional.|1,2,3|
|paginationType|string|The type of interaction that led to the event|next page, previous page, specific page, scroll|
