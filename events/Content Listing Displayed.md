# Content Listing Displayed

Fire whenever a list of content that can or has been searched, filtered, or otherwise dynamically changed is displayed.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Content Listing Displayed",
  "listingDisplayed": {
    "facets": [
      "key|value"
    ],
    "resultsCount": "<resultsCount>",
    "searchTerm": "<searchTerm>",
    "searchType": "<searchType>"
  }
});
```

## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|facets|array|The facets/filters/refinements used in a search|["key\|value", "location\|Brazil", "interests\|analytics"]|
|resultsCount|integer|The total number of items returned that matched the search criteria.|
|searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion.|bluth, blue, red lobster|
|searchType|string|Describes the type of search performed.|article, content, job, people, etc.|