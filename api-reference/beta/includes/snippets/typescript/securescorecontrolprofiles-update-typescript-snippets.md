---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SecureScoreControlProfile();
requestBody.controlStateUpdates = "controlStateUpdates-value";
const result = async () => {
	await graphServiceClient.security.secureScoreControlProfilesById("secureScoreControlProfile-id").patch(requestBody);
}


```