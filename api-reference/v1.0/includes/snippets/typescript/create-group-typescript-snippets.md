---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Group();
requestBody.description = "Self help community for library";
requestBody.displayName = "Library Assist";
requestBody.groupTypes = [
			"Unified"
		]
requestBody.mailEnabled = true;
requestBody.mailNickname = "library";
requestBody.securityEnabled = false;
const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```