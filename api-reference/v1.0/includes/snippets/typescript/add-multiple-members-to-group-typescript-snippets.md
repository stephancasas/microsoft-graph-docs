---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Group();
requestBody.additionalData = {
		 "members@odata.bind" : [
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}",
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}",
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}"
			]
	 }
const result = async () => {
	await graphServiceClient.groupsById("group-id").patch(requestBody);
}


```