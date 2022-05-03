---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ProgramControl();
requestBody.controlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";
requestBody.controlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68";
requestBody.programId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";
const result = async () => {
	await graphServiceClient.programControls.post(requestBody);
}


```