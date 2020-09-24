# Download Link Clicked

Download link clicks will be automatically detected by comparing the href of the link clicked to a predefined list of file extensions. This spec is for manually firing download links if necessary in the future, such as for a button that asynchronously generates the file that will be downloaded using an onClick event.

## Data Attributes HTML Code

```html
  <a href="<linkDestination>" 
    data-layer-eventPrefix="Download Link"
    data-layer-action="click"
    data-layer-category="<category>"
    data-layer-subcategory="<subcategory?>"
    data-layer-fileName="<fileName>" 
    data-layer-reportName="<reportName>"
    data-layer-reportType="<fileType>"
    data-layer-text="<text?>"
  >
```
Items with a ? are optional

## Generated Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Download Link Clicked",
  "linkInfo": {
    "category": "<category>"
    "subcategory": "<subcategory?>"
    "fileName": "<fileName>",
    "linkRegion": "<linkRegion?>",
    "reportName": "<reportName>"
    "reportType": "<fileType>",
    "text": "<text>",
  }
});
```
Items with a ? may not be generated depending on what attributes are present and the ancestry of the clicked item.

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|category|string|Category of the CTA|chat, social, buy now
|subcategory|string|Subcategory of the CTA|facebook, recommended products
|fileName|string|Indicates the filename for download link tracking. Derived from the anchor href attribute|Year End 2012.pdf, Operating Instructions.doc|
|region|string|Pipe-delimited list of all regions in ancestry of clicked item. Automatically generated.|
|linkText|string|Text contents of the item clicked on, or an alternative text label to use instead|Chat with us, Visit our Twitter Page|
|reportName|string|Name of a downloaded file as specified by McKinsey|meet-the-next-normal-consumer|
|reportType|string|Type of a downloaded file. Not the file extension, but rather custom types provided by the site.|pdf, article|