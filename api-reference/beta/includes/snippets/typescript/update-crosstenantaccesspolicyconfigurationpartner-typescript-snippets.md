---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CrossTenantAccessPolicyConfigurationPartner();
requestBody.inboundTrust = new CrossTenantAccessPolicyInboundTrust();
requestBody.inboundTrust.isMfaAccepted = true;
requestBody.inboundTrust.isCompliantDeviceAccepted = true;
requestBody.inboundTrust.isHybridAzureADJoinedDeviceAccepted = true;
const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.partnersById("crossTenantAccessPolicyConfigurationPartner-tenantId").patch(requestBody);
}


```