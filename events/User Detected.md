# User Detected

## Javascript Code

```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Detected",
  "user": {
    "companySize": "<companySize>",
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
|companySize|string|The User Company Size (Employees) variable captures the amount (segmented numerical range) of company employees of a logged-in registered site visitor, based off the self-reported registration information in the logged-in site user's profile.|1-499 employees|
|custKey|string|Set to People Services ID (If a user has a registered mckinsey.com account)
|jobTitle|string|Captures the job title of a logged-in registered site visitor, based off the self-reported registration information in the logged-in site user's profile.|Director/ General Manager|
|loginStatus|string|Describes the login state of the user|logged_in OR logged_out|
|userType|string|Describes the type of the user. Often used to differentiate customers from employees or associates.|employee, guest, agent, customer|
