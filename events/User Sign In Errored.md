# User Sign In Errored

Fire this event when a user attempts to log in but their credentials are incorrect.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Sign In Errored",
});
```