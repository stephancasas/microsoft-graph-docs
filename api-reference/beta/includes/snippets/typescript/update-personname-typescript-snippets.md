---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonName();
requestBody.nickname = "Kesha";
const result = async () => {
	await graphServiceClient.me.profile.namesById("personName-id").patch(requestBody);
}


```