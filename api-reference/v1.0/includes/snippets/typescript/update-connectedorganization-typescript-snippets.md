---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConnectedOrganization();
requestBody.displayName = "Connected organization new name";
requestBody.description = "Connected organization new description";
requestBody.state = ConnectedOrganizationState.Configured;
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizationsById("connectedOrganization-id").patch(requestBody);
}


```