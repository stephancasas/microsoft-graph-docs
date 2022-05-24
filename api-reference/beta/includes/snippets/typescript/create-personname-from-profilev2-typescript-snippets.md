---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonName();
requestBody.displayName = "Innocenty Popov";
requestBody.first = "Innocenty";
requestBody.initials = "IP";
requestBody.last = "Popov";
requestBody.languageTag = "en-US";
requestBody.maiden = null,
const result = async () => {
	await graphServiceClient.me.profile.names.post(requestBody);
}


```