---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GroupLifecyclePolicy();
requestBody.groupLifetimeInDays = 100;
requestBody.managedGroupTypes = "Selected";
requestBody.alternateNotificationEmails = "admin@contoso.com";
const result = async () => {
	await graphServiceClient.groupLifecyclePolicies.post(requestBody);
}


```