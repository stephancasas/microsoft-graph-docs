---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PermissionGrantPolicy();
requestBody.id = "my-custom-consent-policy";
requestBody.displayName = "Custom application consent policy";
requestBody.description = "A custom permission grant policy to customize conditions for granting consent.";
const result = async () => {
	await graphServiceClient.policies.permissionGrantPolicies.post(requestBody);
}


```