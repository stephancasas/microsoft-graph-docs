---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OutlookTask();
requestBody.subject = "Shop for children's weekend";
requestBody.startDateTime = new DateTimeTimeZone();
requestBody.startDateTime.dateTime = "2016-05-03T09:00:00";
requestBody.startDateTime.timeZone = "Eastern Standard Time";
requestBody.dueDateTime = new DateTimeTimeZone();
requestBody.dueDateTime.dateTime = "2016-05-05T16:00:00";
requestBody.dueDateTime.timeZone = "Eastern Standard Time";
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.outlook.tasks.post(requestBody, headers);
}


```