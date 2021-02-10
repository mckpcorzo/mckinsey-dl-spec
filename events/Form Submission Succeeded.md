# Form Submission Succeeded

Fire whenever a form is successfully submitted. Prioritize contact us form as that is the primary one being tracked currently.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Form Submission Succeeded",
  "form": {
    "formID": "<formID>",
    "formName": "<formName>",
    "formType": "<formType>"
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
formID|string|Unique identifier of a form.|F-0113, 2543, CU001, PI-0988|
formName|string|Plain text form name. Generally used if formID is not obtainable. Optional, but preferred if a name is available.|Payment Info, Mailing Address, Payment Address, Contact Us|
|formType|string|Form type used for grouping of similar forms in reports.|profile, registration|