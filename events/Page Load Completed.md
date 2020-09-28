# Page Load Completed

Fire after events for all page load items have been sent.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  'event': 'Page Load Completed',
  'page': {
    "characterLength": "<characterLength>",
  }
})
```

## Variable Definitions

|page.characterLength|integer|The Content Character Length variable counts the number of characters within the body of an I&P page; it is common to get multiple values for this variable due to different browsers. This is also classified into Article Length segments based off an estimated word count (6.7 characters = 1 word); this count is most comparable to the "characters with spaces" count in MS Word. Historical technical implementation here is to count the characters in all html <article> tags on a page.|235, 1742|
