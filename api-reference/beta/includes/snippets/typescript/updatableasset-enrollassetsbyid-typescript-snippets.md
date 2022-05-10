---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EnrollAssetsByIdRequestBody();
requestBody.updateCategory = UpdateCategory.Feature;
requestBody.memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";
requestBody.ids = [
			"String",
			"String",
			"String"
		]
async () => {
	await graphServiceClient.admin.windows.updates.updatableAssets.enrollAssetsById.post(requestBody);
}


```