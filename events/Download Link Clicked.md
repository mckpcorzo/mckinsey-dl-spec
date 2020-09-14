# Download Link Clicked

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Download Link Clicked",
  "linkInfo": {
    "fileName": "<fileName>",
    "reportName": "<reportName>"
    "reportType": "<fileType>",
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|fileName|string|Indicates the filename for download link tracking. Derived from the anchor href attribute|Year End 2012.pdf, Operating Instructions.doc`|
|reportName|string|Name of a downloaded file as specified by McKinsey|meet-the-next-normal-consumer
|reportType|string|Type of a downloaded file. Not the file extension, but rather custom types provided by the site.|pdf, article|