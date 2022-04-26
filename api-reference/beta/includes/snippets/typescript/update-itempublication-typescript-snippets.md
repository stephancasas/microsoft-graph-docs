---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ItemPublication();
requestBody.publisher = "International Association of Branding Management Publishing";
requestBody.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";
const result = async () => {
	await graphServiceClient.usersById("user-id").profile.publicationsById("itemPublication-id").patch(requestBody);
}


```