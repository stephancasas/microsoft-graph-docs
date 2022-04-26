---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AssignTagRequestBody();
requestBody.tenantIds = [
			"String"
		]
const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.tenantTagsById("tenantTag-id").assignTag.post(requestBody);
}


```