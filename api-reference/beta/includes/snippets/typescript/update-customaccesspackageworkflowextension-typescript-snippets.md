---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new 98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0RequestBody();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.customAccessPackageWorkflowExtension",
		 "displayName" : "test_action_0124_email",
		 "description" : "this is for graph testing only"
	 }
async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").customAccessPackageWorkflowExtensionsById("customAccessPackageWorkflowExtension-id").put(requestBody);
}


```