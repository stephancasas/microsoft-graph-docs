---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageAssignmentRequest();
requestBody.requestType = "AdminAdd";
requestBody.accessPackageAssignment = new AccessPackageAssignment();
requestBody.accessPackageAssignment.target = new AccessPackageSubject();
requestBody.accessPackageAssignment.target.email = "user@contoso.com";
requestBody.accessPackageAssignment.assignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8";
requestBody.accessPackageAssignment.accessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(requestBody);
}


```