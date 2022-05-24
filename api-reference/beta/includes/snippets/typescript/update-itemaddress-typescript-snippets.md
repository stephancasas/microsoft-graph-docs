---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ItemAddress();
requestBody.allowedAudiences = AllowedAudiences.Me;
requestBody.displayName = "Secret Hideout";
const result = async () => {
	await graphServiceClient.usersById("user-id").profile.addressesById("itemAddress-id").patch(requestBody);
}


```