---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Event();
requestBody.originalStartTimeZone = "originalStartTimeZone-value";
requestBody.originalEndTimeZone = "originalEndTimeZone-value";
requestBody.responseStatus = new ResponseStatus();
requestBody.responseStatus.response = ResponseType.;
requestBody.responseStatus.time =  new Date("datetime-value");
requestBody.uid = "iCalUId-value";
requestBody.reminderMinutesBeforeStart = 99;
requestBody.isReminderOn = true;
const result = async () => {
	await graphServiceClient.groupsById("group-id").eventsById("event-id").patch(requestBody);
}


```