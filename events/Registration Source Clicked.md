# Registration Source Clicked

This event should be fired whenever a registration link is clicked on?

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Registration Source Clicked",
  "linkInfo": {
    "registrationPageSource": "<registrationPageSource>",
    "registrationSource": "<registrationSource>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|registrationPageSource|The current pageName|home\|mckinsey and company|
|registrationSource|The click region that led user to registration start events|article print header|