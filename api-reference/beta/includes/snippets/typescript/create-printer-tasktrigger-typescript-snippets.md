---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrintTaskTrigger();
requestBody.event = PrintEvent.JobStarted;
requestBody.additionalData = {
		 "definition@odata.bind" : "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
	 }
const result = async () => {
	await graphServiceClient.print.printersById("printer-id").taskTriggers.post(requestBody);
}


```