---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetByIdsRequestBody();
requestBody.ids = [
			"84b80893874940a3-97b7-68513b600544",
			"5d6059b6368d-45f8-91e18e07d485f1d0"
		]
requestBody.types = [
			"user"
		]
const result = async () => {
	await graphServiceClient.directoryObjects.getByIds.post(requestBody);
}


```