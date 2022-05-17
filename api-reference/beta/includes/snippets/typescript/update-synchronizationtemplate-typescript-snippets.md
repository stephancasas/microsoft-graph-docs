---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new {templateId}RequestBody();
requestBody.additionalData = {
		 "id" : "Slack",
		 "applicationId" : "{id}",
		 "factoryTag" : "CustomSCIM"
	 }
const headers = {
	"Authorization": "Bearer <token>",
};
async () => {
	await graphServiceClient.applicationsById("application-id").synchronization.templatesById("synchronizationTemplate-id").put(requestBody, headers);
}


```