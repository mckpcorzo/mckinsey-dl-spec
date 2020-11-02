# Article Saved

Fire when a user saves an article after being prompted to log in.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Article Saved",
});
```