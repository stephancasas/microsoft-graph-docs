---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BaseTaskList();
requestBody.displayName = "Travel Plan";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.taskList"
	 }
const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").patch(requestBody);
}


```