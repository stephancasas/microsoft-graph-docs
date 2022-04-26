---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageAssignmentPolicy();
requestBody.displayName = "New Policy";
requestBody.description = "policy for assignment";
requestBody.allowedTargetScope = AllowedTargetScope.NotSpecified;
requestBody.specificAllowedTargets = [
		]
requestBody.expiration = new ExpirationPattern();
requestBody.expiration.endDateTime = null,
requestBody.expiration.duration = null,
requestBody.expiration.type = ExpirationPatternType.NoExpiration;
requestBody.requestorSettings = new AccessPackageAssignmentRequestorSettings();
requestBody.requestorSettings.enableTargetsToSelfAddAccess = false;
requestBody.requestorSettings.enableTargetsToSelfUpdateAccess = false;
requestBody.requestorSettings.enableTargetsToSelfRemoveAccess = false;
requestBody.requestorSettings.allowCustomAssignmentSchedule = true;
requestBody.requestorSettings.enableOnBehalfRequestorsToAddAccess = false;
requestBody.requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false;
requestBody.requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false;
requestBody.requestorSettings.onBehalfRequestors = [
			]
requestBody.requestApprovalSettings = new AccessPackageAssignmentApprovalSettings();
requestBody.requestApprovalSettings.isApprovalRequiredForAdd = false;
requestBody.requestApprovalSettings.isApprovalRequiredForUpdate = false;
requestBody.requestApprovalSettings.stages = [
			]
requestBody.accessPackage = new AccessPackage();
requestBody.accessPackage.id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentPolicies.post(requestBody);
}


```