# Page Printed

Fire when a user prints a page after being prompted to log in.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Printed",
});
```