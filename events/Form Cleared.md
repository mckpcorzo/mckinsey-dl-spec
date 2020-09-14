# Form Submission Succeeded

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Form Submission Succeeded",
  "form": {
    "formID": "<formID>",
    "formName": "<formName>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
formID|string|Unique identifier of a form.|F-0113, 2543, CU001, PI-0988|
formName|string|Plain text form name. Generally used if formID is not obtainable.|Payment Info, Mailing Address, Payment Address, Contact Us|