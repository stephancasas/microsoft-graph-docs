---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdateAudienceByIdRequestBody();
requestBody.memberEntityType = "String";
requestBody.addMembers = [
			"String"
		]
requestBody.removeMembers = [
			"String"
		]
requestBody.addExclusions = [
			"String"
		]
requestBody.removeExclusions = [
			"String"
		]
async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").audience.updateAudienceById.post(requestBody);
}


```