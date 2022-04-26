---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonInterest();
requestBody.categories = [
			"Sports"
		]
const result = async () => {
	await graphServiceClient.me.profile.interestsById("personInterest-id").patch(requestBody);
}


```