---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddMembersByIdRequestBody();
requestBody.ids = [
			"String",
			"String",
			"String"
		]
requestBody.memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";
async () => {
	await graphServiceClient.admin.windows.updates.updatableAssetsById("updatableAsset-id").addMembersById.post(requestBody);
}


```