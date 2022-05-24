---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChangeDeploymentStatusRequestBody();
requestBody.tenantGroupId = "String";
requestBody.tenantId = "String";
requestBody.managementActionId = "String";
requestBody.managementTemplateId = "String";
requestBody.status = "String";
const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.managementActionTenantDeploymentStatuses.changeDeploymentStatus.post(requestBody);
}


```