---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CheckMemberGroupsRequestBody();
requestBody.groupIds = [
			"fee2c45b-915a-4a64b130f4eb9e75525e",
			"4fe90ae065a-478b9400e0a0e1cbd540"
		]
const result = async () => {
	await graphServiceClient.me.checkMemberGroups.post(requestBody);
}


```