# Password Reset Started

Fire when a user starts the password reset process, usually by requesting a reset email

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Password Reset Started",
});
```