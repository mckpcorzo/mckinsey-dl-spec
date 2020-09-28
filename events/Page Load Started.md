# Page Load Started

This should be the first event to fire on most pages. Sets page-level variables that will be sent to analytics on Page Load Completed.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
  "page": {
    "contentType": "<contentType>",
    "daysSinceLastPublish": "<daysSinceLastPublish>",
    "displayDate": "<displayDate>",
    "editorialMonthPublicationDate": "<editorialMonthPublicationDate>",
    "domain": "<domain>",
    "pageName": "<pageName>",
    "pageTitle": "<pageTitle>",
    "siteCoreId": "<siteCoreId>",
    "subsection": "<subsection>",
    "subsection2": "<subsection2>",
    "subsection3": "<subsection3>",
    "subsection4": "<subsection4>",
    "subsection5": "<subsection5>"
  },
  "article": {
    "source": "<source>"
  }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|article.source|string|The Publishing Source variable captures the publishing source of a piece of content (McKinsey Quarterly, MGI, etc.); if a value isn't available, the default value is set to "McKinsey Generic."|
|page.contentType|string|The template used by type|Article, Home, Careers, etc|
|page.daysSinceLastPublish|string|The Days Since CMS Publication variable captures the number of days since the page was published live onto the site. This variable may have multiple entries; choose the largest value.|
|page.displayDate|string|The Display Date variable captures the date when a page or piece of content was last published to the site per SiteCore CMS|
|page.editorialMonthPublicationDate|string|The Editorial Month Publication Date variable captures the date, from the SiteCore CMS, when a piece of content was published onto the site.|
|page.domain|string|Captures the root domain folder (the ".com") of the URL. Example: http://www.mckinsey.com/insights/marketing_sales/five_ways_to_get_more_from_digital_advertising; here, Site Section 1 is www.mckinsey.com.|
|page.pageName|string|The Page Name variable is a copy of the Page value.|
|page.pageTitle|string|The Page Title variable captures what is displayed at the very top of a user's web browser (in the tab). Currently set to JS value document.title.|
|page.siteCoreId|string|The SiteCore ID variable captures the ID # of the web page from the SiteCore CMS, if SiteCore was used to publish the content.|
|page.subsection|string|The Site Section 2 variable captures the site section (1st subfolder of  the URL), with the exception of the site home page, which is set to "McKinsey Dotcom Home_Page." Site Section 2 is used to analyze site section Pathing via the Paths > Site Section 2 report. Example: http://www.mckinsey.com/insights/marketing_sales/five_ways_to_get_more_from_digital_advertising; here, Site Section 2 is insights.|insights|
|page.subsection2|string|The Site Section 3 variable captures the 2nd subfolder of the site URL after the root domain folder. Example: http://www.mckinsey.com/insights/marketing_sales/five_ways_to_get_more_from_digital_advertising; here, Site Section 3 is marketing_sales.|marketing_sales|
|page.subsection3|string|The Site Section 4 variable captures the 3rd subfolder of the site URL after the root domain folder. Example: http://www.mckinsey.com/insights/marketing_sales/five_ways_to_get_more_from_digital_advertising; here, Site Section 4 is five_ways_to_get_more_from_digital_advertising.|five_ways_to_get_more_from_digital_advertising|
|page.subsection4|string|The Site Section 5 variable captures the 4th subfolder of the site URL after the root domain folder. Example: http://www.mckinsey.com/careers/create_your_path/career_pathways/career_pathways_advanced_degrees; here, Site Section 5 is career_pathways_advanced_degrees.|career_pathways_advanced_degrees|
|page.subsection5|string|The Site Section 6 variable captures the 5th subfolder of the site URL after the root domain folder. Example: http://www.mckinsey.com/global_locations/asia/japan/ja/our_people; here, Site Section 6 is our_people.|our_people|