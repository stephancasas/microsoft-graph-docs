---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddCopyFromContentTypeHubRequestBody();
requestBody.contentTypeId = "0x0101";
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").contentTypes.addCopyFromContentTypeHub.post(requestBody);
}


```