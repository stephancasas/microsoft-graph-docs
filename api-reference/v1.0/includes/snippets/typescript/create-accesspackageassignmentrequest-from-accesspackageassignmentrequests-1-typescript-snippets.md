---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageAssignmentRequest();
requestBody.requestType = AccessPackageRequestType.AdminAdd;
requestBody.assignment = new AccessPackageAssignment();
requestBody.assignment.additionalData = {
			 "targetId" : "46184453-e63b-4f20-86c2-c557ed5d5df9",
			 "assignmentPolicyId" : "2264bf65-76ba-417b-a27d-54d291f0cbc8",
			 "accessPackageId" : "a914b616-e04e-476b-aa37-91038f0b165b"
		 }
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentRequests.post(requestBody);
}


```