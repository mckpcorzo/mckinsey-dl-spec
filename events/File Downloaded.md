# File Downloaded

Fire when a user downloads a file after being prompted to log in.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "File Downloaded",
});
```