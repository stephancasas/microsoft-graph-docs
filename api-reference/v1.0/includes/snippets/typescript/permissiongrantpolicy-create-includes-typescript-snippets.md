---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PermissionGrantConditionSet();
requestBody.permissionType = PermissionType.Delegated;
requestBody.clientApplicationsFromVerifiedPublisherOnly = true;
const result = async () => {
	await graphServiceClient.policies.permissionGrantPoliciesById("permissionGrantPolicy-id").includes.post(requestBody);
}


```