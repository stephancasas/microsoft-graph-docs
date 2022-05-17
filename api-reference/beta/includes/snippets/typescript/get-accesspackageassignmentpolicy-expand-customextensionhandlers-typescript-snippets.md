---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "customExtensionHandlers($expand=customExtension)",
};
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPoliciesById("accessPackageAssignmentPolicy-id").get(requestParameters);
}


```