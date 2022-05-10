---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddMembersRequestBody();
const updatableasset = new UpdatableAsset();
updatableasset.additionalData = {
					 "@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
					 "id" : "String (identifier)"
				 }
requestBody.assets = [
			updatableasset
		]
async () => {
	await graphServiceClient.admin.windows.updates.updatableAssetsById("updatableAsset-id").addMembers.post(requestBody);
}


```