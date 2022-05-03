---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRequest();
requestBody.catalogId = "beedadfe-01d5-4025-910b-84abb9369997";
requestBody.requestType = "AdminRemove";
requestBody.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResource.id = "354078e5-dbce-4894-8af4-0ab274d41662";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```