---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SetUserPreferredPresenceRequestBody();
requestBody.availability = "DoNotDisturb";
requestBody.activity = "DoNotDisturb";
requestBody.expirationDuration = "PT8H";
async () => {
	await graphServiceClient.usersById("user-id").presence.setUserPreferredPresence.post(requestBody);
}


```