---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OutlookTaskFolder();
requestBody.name = "Charity work";
const result = async () => {
	await graphServiceClient.me.outlook.taskFoldersById("outlookTaskFolder-id").patch(requestBody);
}


```