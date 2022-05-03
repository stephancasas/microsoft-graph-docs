---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Event();
requestBody.location = new Location();
requestBody.location.displayName = "Conf Room 2";
const result = async () => {
	await graphServiceClient.groupsById("group-id").calendar.eventsById("event-id").patch(requestBody);
}


```