---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdatableAsset();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.windowsUpdates.updatableAssetGroup"
	 }
const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssets.post(requestBody);
}


```