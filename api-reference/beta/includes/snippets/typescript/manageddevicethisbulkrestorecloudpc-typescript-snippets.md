---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BulkRestoreCloudPcRequestBody();
requestBody.managedDeviceIds = [
			"30d0e128-de93-41dc-89ec-33d84bb662a0",
			"7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
		]
requestBody.restorePointDateTime =  new Date("2021-09-23T04:00:00.0000000");
requestBody.timeRange = RestoreTimeRange.Before;
const result = async () => {
	await graphServiceClient.deviceManagement.managedDevices.bulkRestoreCloudPc.post(requestBody);
}


```