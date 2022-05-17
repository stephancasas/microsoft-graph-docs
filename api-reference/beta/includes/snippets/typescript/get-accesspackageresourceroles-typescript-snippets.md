---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "(originSystem%20eq%20'AadGroup'%20and%20accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')",
	expand : "accessPackageResource",
};
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").accessPackageResourceRoles.get(requestParameters);
}


```