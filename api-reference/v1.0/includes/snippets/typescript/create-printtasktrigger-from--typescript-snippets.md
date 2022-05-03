---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrintTaskTrigger();
requestBody.event = PrintEvent.JobStarted;
requestBody.additionalData = {
		 "definition@odata.bind" : "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
	 }
const result = async () => {
	await graphServiceClient.print.printersById("printer-id").taskTriggers.post(requestBody);
}


```