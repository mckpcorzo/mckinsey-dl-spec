# User Unsubscribed

Fire whenever a user unsubscribes from a campaign or information source.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Unsubscribed",
  "subscription": {
    "subscriptionType": "<subscriptionType>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|subscriptionType|string|Describes the type of subscription.|news, updates, sales, events, rss|