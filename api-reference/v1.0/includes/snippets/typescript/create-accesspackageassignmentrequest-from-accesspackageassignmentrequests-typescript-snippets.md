---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageAssignmentRequest();
requestBody.requestType = AccessPackageRequestType.UserAdd;
requestBody.assignment = new AccessPackageAssignment();
requestBody.assignment.additionalData = {
			 "accessPackageId" : "d7be3253-b9c6-4fab-adef-30d30de8da2b"
		 }
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentRequests.post(requestBody);
}


```