---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OutlookTaskGroup();
requestBody.name = "Leisure tasks";
const result = async () => {
	await graphServiceClient.me.outlook.taskGroups.post(requestBody);
}


```