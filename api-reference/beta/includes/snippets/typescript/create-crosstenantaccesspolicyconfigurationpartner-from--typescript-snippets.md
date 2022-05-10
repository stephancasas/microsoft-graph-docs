---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CrossTenantAccessPolicyConfigurationPartner();
requestBody.tenantId = "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a";
requestBody.b2bDirectConnectOutbound = new CrossTenantAccessPolicyB2BSetting();
requestBody.b2bDirectConnectOutbound.usersAndGroups = new CrossTenantAccessPolicyTargetConfiguration();
requestBody.b2bDirectConnectOutbound.usersAndGroups.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Blocked;
const crosstenantaccesspolicytarget = new CrossTenantAccessPolicyTarget();
crosstenantaccesspolicytarget.additionalData = {
							 "target" : "6f546279-4da5-4b53-a095-09ea0cef9971",
							 "targetType" : "group"
						 }
requestBody.b2bDirectConnectOutbound.usersAndGroups.targets = [
					crosstenantaccesspolicytarget
				]
requestBody.b2bDirectConnectInbound = new CrossTenantAccessPolicyB2BSetting();
requestBody.b2bDirectConnectInbound.applications = new CrossTenantAccessPolicyTargetConfiguration();
requestBody.b2bDirectConnectInbound.applications.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.Allowed;
const crosstenantaccesspolicytarget = new CrossTenantAccessPolicyTarget();
crosstenantaccesspolicytarget.additionalData = {
							 "target" : "Office365",
							 "targetType" : "application"
						 }
requestBody.b2bDirectConnectInbound.applications.targets = [
					crosstenantaccesspolicytarget
				]
const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.partners.post(requestBody);
}


```