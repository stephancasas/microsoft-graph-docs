---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AppManagementPolicy();
requestBody.isEnabled = false;
const result = async () => {
	await graphServiceClient.policies.appManagementPoliciesById("appManagementPolicy-id").patch(requestBody);
}


```