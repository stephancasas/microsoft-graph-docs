---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonWebsite();
requestBody.categories = [
			"football"
		]
requestBody.displayName = "Lyn Damer";
requestBody.webUrl = "www.lyndamer.no";
const result = async () => {
	await graphServiceClient.me.profile.websites.post(requestBody);
}


```