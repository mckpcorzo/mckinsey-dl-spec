# MailTo Link Clicked

Fire whenever a mailto link is clicked. 

Prioritize this last as it may change.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "MailTo Link Clicked",
});
```