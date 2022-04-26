---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChangeScreenSharingRoleRequestBody();
requestBody.role = ScreenSharingRole.Viewer;
async () => {
	await graphServiceClient.communications.callsById("call-id").changeScreenSharingRole.post(requestBody);
}


```