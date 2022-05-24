---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdateAudienceRequestBody();
const updatableasset = new UpdatableAsset();
updatableasset.additionalData = {
					 "@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
					 "id" : "String (identifier)"
				 }
requestBody.addMembers = [
			updatableasset
		]
const updatableasset = new UpdatableAsset();
updatableasset.additionalData = {
					 "@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
					 "id" : "String (identifier)"
				 }
requestBody.removeMembers = [
			updatableasset
		]
const updatableasset = new UpdatableAsset();
updatableasset.additionalData = {
					 "@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
					 "id" : "String (identifier)"
				 }
requestBody.addExclusions = [
			updatableasset
		]
const updatableasset = new UpdatableAsset();
updatableasset.additionalData = {
					 "@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
					 "id" : "String (identifier)"
				 }
requestBody.removeExclusions = [
			updatableasset
		]
async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").audience.updateAudience.post(requestBody);
}


```