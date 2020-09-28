# McKinsey Data Layer and Data Attribute Spec

## Overview
This repository contains the necessary specifications to build an Event Driven Data Layer.

## Data Layer
Each file inside the **[events](events)** folder corresponds to a single use case or site event that needs to be implemented.

These will be used to share data with the tag management tool of choice and to trigger the corresponding tracking events in the analytics tool of choice.

## Data Attributes
Custom HTML data attributes enable some data layer events to be fired without developers having to write Javascript to fire them. They are added to the HTML source code on specific page elements so that interactions with those elements can be tracked. They are most often used for custom click events, though they can also be used for hover events, form field changes, form submissions, and many other similar Javascript events.

### Region attribute
The data-layer-region click attribute is unique in that it is used by all data attribute custom events. It should be applied to the HTML elements for each possible region of the page/site that needs to be tracked. 

For instance, the main page <header> tag might have the data-layer-region="header" attribute added to it. Any data layer events that are triggered via interactions with child HTML elements under this <header> that have their 

## Questions/Comments
For any questions or comments, please contact cory.watson@searchdiscovery.com.