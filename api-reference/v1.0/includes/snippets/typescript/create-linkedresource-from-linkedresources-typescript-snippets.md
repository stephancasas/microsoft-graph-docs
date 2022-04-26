---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new LinkedResource();
requestBody.webUrl = "https://microsoft.com";
requestBody.applicationName = "Microsoft";
requestBody.displayName = "Microsoft";
requestBody.externalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9";
const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasksById("todoTask-id").linkedResources.post(requestBody);
}


```