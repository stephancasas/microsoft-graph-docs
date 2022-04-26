---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AppRoleAssignment();
requestBody.principalId = "33ad69f9-da99-4bed-acd0-3f24235cb296";
requestBody.resourceId = "9028d19c-26a9-4809-8e3f-20ff73e2d75e";
requestBody.appRoleId = "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7";
const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").appRoleAssignedTo.post(requestBody);
}


```