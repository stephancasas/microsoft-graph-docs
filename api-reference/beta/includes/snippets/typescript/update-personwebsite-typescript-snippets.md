---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonWebsite();
requestBody.description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway";
const result = async () => {
	await graphServiceClient.me.profile.websitesById("personWebsite-id").patch(requestBody);
}


```