---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CrossTenantAccessPolicyConfigurationDefault();
requestBody.b2bCollaborationOutbound = new CrossTenantAccessPolicyB2BSetting();
requestBody.b2bCollaborationOutbound.usersAndGroups = new CrossTenantAccessPolicyTargetConfiguration();
requestBody.b2bCollaborationOutbound.usersAndGroups.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked;
const crosstenantaccesspolicytarget = new CrossTenantAccessPolicyTarget();
crosstenantaccesspolicytarget.additionalData = {
							 "target" : "0be493dc-cb56-4a53-936f-9cf64410b8b0",
							 "targetType" : "group"
						 }
requestBody.b2bCollaborationOutbound.usersAndGroups.targets = [
					crosstenantaccesspolicytarget
				]
requestBody.b2bCollaborationOutbound.applications = new CrossTenantAccessPolicyTargetConfiguration();
requestBody.b2bCollaborationOutbound.applications.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked;
const crosstenantaccesspolicytarget = new CrossTenantAccessPolicyTarget();
crosstenantaccesspolicytarget.additionalData = {
							 "target" : "AllApplications",
							 "targetType" : "application"
						 }
requestBody.b2bCollaborationOutbound.applications.targets = [
					crosstenantaccesspolicytarget
				]
const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.default.patch(requestBody);
}


```