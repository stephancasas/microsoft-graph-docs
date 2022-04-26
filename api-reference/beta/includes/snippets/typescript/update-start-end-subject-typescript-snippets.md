---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OnlineMeeting();
requestBody.startDateTime =  new Date("2020-09-09T14:33:30.8546353-07:00");
requestBody.endDateTime =  new Date("2020-09-09T15:03:30.8566356-07:00");
requestBody.subject = "Patch Meeting Subject";
const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").patch(requestBody);
}


```