---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageCatalog();
requestBody.displayName = "sales";
requestBody.description = "for employees working with sales and outside sales partners";
requestBody.isExternallyVisible = true;
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogs.post(requestBody);
}


```