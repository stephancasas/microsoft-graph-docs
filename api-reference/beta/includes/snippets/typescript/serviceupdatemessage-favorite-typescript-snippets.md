---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new FavoriteRequestBody();
requestBody.messageIds = [
			"MC172851",
			"MC167983"
		]
const result = async () => {
	await graphServiceClient.admin.serviceAnnouncement.messages.favorite.post(requestBody);
}


```