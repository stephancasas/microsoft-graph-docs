---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Permission();
requestBody.roles = [
			"read"
		]
const result = async () => {
	await graphServiceClient.sitesById("site-id").permissionsById("permission-id").patch(requestBody);
}


```