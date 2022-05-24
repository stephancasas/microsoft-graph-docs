---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TenantTag();
requestBody.displayName = "Support";
requestBody.description = "Tenants that have purchased extended support";
const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.tenantTags.post(requestBody);
}


```