# User Signed Out

Fire whenever a user signs out of their account on the site.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Signed Out",
});
```