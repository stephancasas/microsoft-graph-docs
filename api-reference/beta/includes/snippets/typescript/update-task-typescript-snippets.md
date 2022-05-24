---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrintTask();
requestBody.status = new PrintTaskStatus();
requestBody.status.state = PrintTaskProcessingState.Completed;
requestBody.status.description = "completed";
const result = async () => {
	await graphServiceClient.print.taskDefinitionsById("printTaskDefinition-id").tasksById("printTask-id").patch(requestBody);
}


```