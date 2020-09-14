# Page Load Completed

Fire after events for all page load items have been sent.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  'event': 'Page Load Completed'
})
```