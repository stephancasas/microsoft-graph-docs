---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRequest();
requestBody.catalogId = "beedadfe-01d5-4025-910b-84abb9369997";
requestBody.requestType = "AdminAdd";
requestBody.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResource.originId = "c6294667-7348-4f5a-be73-9d2c65f574f3";
requestBody.accessPackageResource.originSystem = "AadGroup";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```