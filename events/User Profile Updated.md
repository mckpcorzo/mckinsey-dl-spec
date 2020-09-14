# User Profile Updated

Fire whenever a user updates their account profile. Could be replaced by Form Submission Succeeded depending on the context.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Profile Updated"
});
```