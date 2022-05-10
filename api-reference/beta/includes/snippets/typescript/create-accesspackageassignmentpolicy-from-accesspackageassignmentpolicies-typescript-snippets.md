---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageAssignmentPolicy();
requestBody.accessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d";
requestBody.displayName = "direct";
requestBody.description = "direct assignments by administrator";
requestBody.accessReviewSettings = null,
requestBody.requestorSettings = new RequestorSettings();
requestBody.requestorSettings.scopeType = "NoSubjects";
requestBody.requestorSettings.acceptRequests = true;
requestBody.requestorSettings.allowedRequestors = [
			]
requestBody.requestApprovalSettings = new ApprovalSettings();
requestBody.requestApprovalSettings.isApprovalRequired = false;
requestBody.requestApprovalSettings.isApprovalRequiredForExtension = false;
requestBody.requestApprovalSettings.isRequestorJustificationRequired = false;
requestBody.requestApprovalSettings.approvalMode = "NoApproval";
requestBody.requestApprovalSettings.approvalStages = [
			]
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(requestBody);
}


```