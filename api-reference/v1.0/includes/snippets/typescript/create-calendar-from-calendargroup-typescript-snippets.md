---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Calendar();
requestBody.name = "Marketing calendar";
const result = async () => {
	await graphServiceClient.me.calendarGroupsById("calendarGroup-id").calendars.post(requestBody);
}


```