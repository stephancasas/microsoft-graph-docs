---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "originSystem%20eq%20'SharePointOnline'",
};
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceEnvironments.get(requestParameters);
}


```