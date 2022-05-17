---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CalendarGroup();
requestBody.name = "Personal events";
const result = async () => {
	await graphServiceClient.me.calendarGroups.post(requestBody);
}


```