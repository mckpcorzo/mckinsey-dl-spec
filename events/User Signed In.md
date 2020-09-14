# User Signed In

Fire whenever a user successfully signs in to their account on the site.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Signed In",
});
```