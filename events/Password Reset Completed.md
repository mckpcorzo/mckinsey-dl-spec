# Password Reset Started

Fire when a user completes the password reset process, usually by submitting a new password successfully

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Password Reset Completed",
});
```