---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'Directory'",
};
const result = async () => {
	await graphServiceClient.policies.roleManagementPolicyAssignments.get(requestParameters);
}


```