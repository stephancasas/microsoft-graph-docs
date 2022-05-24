---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "(originSystem%20eq%20'SharePointOnline'%20and%20accessPackageResource/id%20eq%20'53c71803-a0a8-4777-aecc-075de8ee3991')",
	select : "displayName,originId",
};
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").accessPackageResourceRoles.get(requestParameters);
}


```