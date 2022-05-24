---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ItemPhone();
requestBody.displayName = "Car Phone";
requestBody.number = "+7 499 342 22 13";
const result = async () => {
	await graphServiceClient.me.profile.phones.post(requestBody);
}


```