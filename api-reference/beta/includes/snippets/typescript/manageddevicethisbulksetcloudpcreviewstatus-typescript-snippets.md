---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BulkSetCloudPcReviewStatusRequestBody();
requestBody.managedDeviceIds = [
			"30d0e128-de93-41dc-89ec-33d84bb662a0",
			"7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
		]
requestBody.reviewStatus = new CloudPcReviewStatus();
requestBody.reviewStatus.inReview = true;
requestBody.reviewStatus.userAccessLevel = CloudPcUserAccessLevel.Restricted;
requestBody.reviewStatus.azureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview";
const result = async () => {
	await graphServiceClient.deviceManagement.managedDevices.bulkSetCloudPcReviewStatus.post(requestBody);
}


```