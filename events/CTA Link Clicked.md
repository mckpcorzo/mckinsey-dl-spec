# CTA Link Clicked

## Data Attributes HTML Code

```html
  <a href="<linkDestination>"
    data-layer-eventPrefix="CTA Link"
    data-layer-action="click"
    data-layer-linkInfo-category="<category>"
    data-layer-linkInfo-subcategory="<subcategory?>"
    data-layer-linkInfo-subcategory2="<subcategory2?>"
    data-layer-linkInfo-text="<linkText?>"
  >
```

Items with a ? are optional

## Generated Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "CTA Link Clicked",
  "linkInfo": {
    "category": "<category>",
    "subcategory": "<subcategory?>",
    "subcategory2": "<subcategory2?>",
    "region": "<region?>",
    "text": "<text>",
  }
});
```

Items with a ? may not be generated depending on what attributes are present and the ancestry of the clicked item.

### Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|category|string|Category of the CTA|chat, ecommerce, learn more, share, subscribe, visit|
|subcategory|string|Subcategory of the CTA link|buy now, email, print, social|
|subcategory2|string|Subcategory tier 2 of the CTA link. Often used for service names, such as with a share > social.|facebook, twitter|
|region|string|Pipe-delimited list of all regions in ancestry of clicked item. Automatically generated.|
|text|string|Text contents of the item clicked on, or an alternative text label to use instead|Chat with us, Visit our Twitter Page|