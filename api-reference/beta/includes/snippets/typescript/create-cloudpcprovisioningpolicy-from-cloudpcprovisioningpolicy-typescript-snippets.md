---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcProvisioningPolicy();
requestBody.description = "Description value";
requestBody.displayName = "Display Name value";
requestBody.domainJoinConfiguration = new CloudPcDomainJoinConfiguration();
requestBody.domainJoinConfiguration.onPremisesConnectionId = "16ee6c71-fc10-438b-88ac-daa1ccafffff";
requestBody.domainJoinConfiguration.additionalData = {
			 "domainJoinType" : "hybridAzureADJoin"
		 }
requestBody.id = "1d164206-bf41-4fd2-8424-a3192d39ffff";
requestBody.imageDisplayName = "Windows-10 19h1-evd";
requestBody.imageId = "MicrosoftWindowsDesktop_Windows-10_19h1-evd";
requestBody.imageType = CloudPcProvisioningPolicyImageType.Gallery;
requestBody.onPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff";
requestBody.windowsSettings = new CloudPcWindowsSettings();
requestBody.windowsSettings.language = "en-US";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcProvisioningPolicy"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.provisioningPolicies.post(requestBody);
}


```