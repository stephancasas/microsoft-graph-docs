---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ServicePrincipal();
requestBody.appRoleAssignmentRequired = true;
const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").patch(requestBody);
}


```