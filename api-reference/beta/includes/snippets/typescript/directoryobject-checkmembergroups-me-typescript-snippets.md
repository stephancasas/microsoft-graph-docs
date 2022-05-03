---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CheckMemberGroupsRequestBody();
requestBody.groupIds = [
			"fee2c45b-915a-4a64-b130-f4eb9e75525e",
			"4fe90ae7-065a-478b-9400-e0a0e1cbd540"
		]
const result = async () => {
	await graphServiceClient.me.checkMemberGroups.post(requestBody);
}


```