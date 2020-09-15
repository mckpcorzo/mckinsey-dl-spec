# Registration Source Clicked

Fire whenever a link directing a user to register is clicked on. It is used to populate a cookie to track registration source. Prioritize this last as it may change.

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

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|registrationPageSource|string|The current pageName|home\|mckinsey and company|
|registrationSource|string|The click region that led user to registration start events|article print header|