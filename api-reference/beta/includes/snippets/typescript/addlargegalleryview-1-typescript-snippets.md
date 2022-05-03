---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddLargeGalleryViewRequestBody();
requestBody.clientContext = "785f4929-92ca-497b-863f-c778c77c9758";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").addLargeGalleryView.post(requestBody);
}


```