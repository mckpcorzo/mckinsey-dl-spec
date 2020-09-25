# Navigation Link Clicked

This is the fallback event that will be sent if an HTML anchor link is clicked and no other more specialized click event is triggered (cta, download, exit, etc). The data attribute spec enables manually overriding the more specialized clicks to classify a link as simple navigation.

## Data Attributes HTML Code

```html
  <a href="<linkDestination>"
    data-layer-eventPrefix="Navigation Link"
    data-layer-action="click"
    data-layer-linkInfo-linkInfo-category="<category>"
    data-layer-linkInfo-linkInfo-subcategory="<subcategory?>"
    data-layer-linkInfo-linkInfo-text="<linkText?>"
  >
```

Items with a ? are optional

## Generated Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Navigation Link Clicked",
  "linkInfo": {
    "category": "<category>"
    "subcategory": "<subcategory?>"
    "region": "<region?>",
    "text": "<text>",
  }
});
```

Items with a ? may not be generated depending on what attributes are present and the ancestry of the clicked item.

### Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|category|string|Additional subtype of the CTA|facebook|
|region|string|Pipe-delimited list of all regions in ancestry of clicked item. Automatically generated.|
|subcategory|string|Subcategory of the exit link|chat, social, buy now|
|text|string|Text contents of the item clicked on, or an alternative text label to use instead|Chat with us, Visit our Twitter Page|