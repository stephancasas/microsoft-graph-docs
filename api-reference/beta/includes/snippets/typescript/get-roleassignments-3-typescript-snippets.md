---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "appScopeId%20eq%20'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'",
	expand : "principal",
};
const result = async () => {
	await graphServiceClient.roleManagement.entitlementManagement.roleAssignments.get(requestParameters);
}


```