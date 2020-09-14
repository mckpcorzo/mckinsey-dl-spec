# User Detected

Fire between page load started and page load completed when user information is available.

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Detected",
  "user": {
    "companyName": "<companyName>",
    "custKey": "<custKey>",
    "jobTitle": "<jobTitle>",
    "loginStatus": "<loginStatus>",
    "userType": "<userType>"
  }
});
```
## Variable Definitions

|Field|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|companyName|string|The User Company Name|McKinsey & Company|
|custKey|string|Set to People Services ID (If a user has a registered mckinsey.com account)
|jobTitle|string|Captures the job title of a logged-in registered site visitor, based off the self-reported registration information in the logged-in site user's profile.|Director/ General Manager|
|loginStatus|string|Describes the login state of the user|logged_in OR logged_out|
|userType|string|Describes the type of the user. Often used to differentiate customers from employees or associates.|employee, guest, agent, customer|
