# Content Listing Displayed

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Listing Displayed",
  "listingDisplayed": {
    "facets": "<facets>", // Need to determine how these are tracked
    "refinements": "<refinements>", // Need to determine how these are tracked
    "resultsCount": "<resultsCount>"
    "searchTerm": "<searchTerm>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|facets|array|The facets used in the search|
|refinements|array|The refinements used in the search|
|resultsCount|integer|The total number of items returned that matched the search criteria.|
|searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion.|bluth, blue, red lobster|
|searchType|string|Describes the domain of the search.|products, properties, articles, authors, coupons, publications|