---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ResizeCloudPcRequestBody();
requestBody.targetServicePlanId = "30d0e128-de93-41dc-89ec-33d84bb662a0";
async () => {
	await graphServiceClient.deviceManagement.managedDevicesById("managedDevice-id").resizeCloudPc.post(requestBody);
}


```