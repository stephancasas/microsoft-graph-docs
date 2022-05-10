---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "resourceType%20eq%20'Application'",
	expand : "accessPackageResourceScopes",
};
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").accessPackageResources.get(requestParameters);
}


```