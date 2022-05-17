---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcDeviceImage();
requestBody.displayName = "Display Name value";
requestBody.osBuildNumber = "OS Build Number value";
requestBody.operatingSystem = "Operating System value";
requestBody.version = "Version value";
requestBody.sourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcDeviceImage"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.deviceImages.post(requestBody);
}


```