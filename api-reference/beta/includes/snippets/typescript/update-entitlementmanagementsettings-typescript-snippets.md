---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EntitlementManagementSettings();
requestBody.externalUserLifecycleAction = "None";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.settings.patch(requestBody);
}


```