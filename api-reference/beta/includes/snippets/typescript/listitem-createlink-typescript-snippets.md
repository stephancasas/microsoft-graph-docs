---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateLinkRequestBody();
requestBody.type = "embed";
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").itemsById("listItem-id").createLink.post(requestBody);
}


```