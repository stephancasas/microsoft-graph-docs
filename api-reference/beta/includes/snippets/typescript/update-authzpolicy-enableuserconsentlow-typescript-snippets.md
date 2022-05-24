---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthorizationPolicy();
requestBody.permissionGrantPolicyIdsAssignedToDefaultUserRole = [
			"managePermissionGrantsForSelf.microsoft-user-default-low"
		]
const result = async () => {
	await graphServiceClient.policies.authorizationPolicyById("authorizationPolicy-id").patch(requestBody);
}


```