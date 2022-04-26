---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SelfActivateRequestBody();
requestBody.reason = "reason-value";
requestBody.duration = "duration-value";
requestBody.ticketNumber = "ticketNumber-value";
requestBody.ticketSystem = "ticketSystem-value";
const result = async () => {
	await graphServiceClient.privilegedRolesById("privilegedRole-id").selfActivate.post(requestBody);
}


```