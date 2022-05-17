---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcProvisioningPolicy();
requestBody.displayName = "HR provisioning policy";
requestBody.description = "Provisioning policy for India HR employees";
requestBody.onPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff";
requestBody.imageId = "Image ID value";
requestBody.imageDisplayName = "Image Display Name value";
requestBody.imageType = CloudPcProvisioningPolicyImageType.Custom;
requestBody.windowsSettings = new CloudPcWindowsSettings();
requestBody.windowsSettings.language = "en-US";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcProvisioningPolicy"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.provisioningPoliciesById("cloudPcProvisioningPolicy-id").patch(requestBody);
}


```