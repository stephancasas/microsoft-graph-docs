---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Group();
requestBody.description = "Contoso Life v2.0";
requestBody.displayName = "Contoso Life Renewed";
const result = async () => {
	await graphServiceClient.groupsById("group-id").patch(requestBody);
}


```