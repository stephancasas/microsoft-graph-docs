---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SynchronizationTemplate();
requestBody.id = "SCIM-Test1";
requestBody.applicationId = "{id}";
requestBody.factoryTag = "CustomSCIM";
const result = async () => {
	await graphServiceClient.applicationsById("application-id").synchronization.templates.post(requestBody);
}


```