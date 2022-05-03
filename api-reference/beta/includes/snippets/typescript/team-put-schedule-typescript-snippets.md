---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ScheduleRequestBody();
requestBody.additionalData = {
		 "enabled" : true,
		 "timeZone" : "America/Chicago"
	 }
async () => {
	await graphServiceClient.teamsById("team-id").schedule.put(requestBody);
}


```