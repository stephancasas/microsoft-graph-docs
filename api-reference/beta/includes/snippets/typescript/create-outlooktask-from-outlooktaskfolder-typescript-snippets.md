---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OutlookTask();
requestBody.subject = "Shop for dinner";
requestBody.startDateTime = new DateTimeTimeZone();
requestBody.startDateTime.dateTime = "2016-04-23T18:00:00";
requestBody.startDateTime.timeZone = "Pacific Standard Time";
requestBody.dueDateTime = new DateTimeTimeZone();
requestBody.dueDateTime.dateTime = "2016-04-25T13:00:00";
requestBody.dueDateTime.timeZone = "Pacific Standard Time";
const result = async () => {
	await graphServiceClient.me.outlook.taskFoldersById("outlookTaskFolder-id").tasks.post(requestBody);
}


```