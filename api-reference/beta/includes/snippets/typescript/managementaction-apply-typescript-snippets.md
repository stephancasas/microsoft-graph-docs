---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ApplyRequestBody();
requestBody.tenantId = "String";
requestBody.tenantGroupId = "String";
requestBody.managementTemplateId = "String";
const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.managementActionsById("managementAction-id").apply.post(requestBody);
}


```