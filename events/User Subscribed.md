# User Subscribed

Fire whenever a user subscribes to a campaign or information source.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Subscribed",
  "subscription": {
    "subscriptionType": "<subscriptionType>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|subscriptionType|string|Describes the type of subscription.|news, updates, sales, events, rss|