---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SetCloudPcReviewStatusRequestBody();
requestBody.reviewStatus = new CloudPcReviewStatus();
requestBody.reviewStatus.inReview = true;
requestBody.reviewStatus.userAccessLevel = CloudPcUserAccessLevel.Restricted;
requestBody.reviewStatus.azureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview";
async () => {
	await graphServiceClient.deviceManagement.managedDevicesById("managedDevice-id").setCloudPcReviewStatus.post(requestBody);
}


```