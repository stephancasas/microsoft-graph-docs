---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddCopyRequestBody();
requestBody.contentType = "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101";
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").contentTypes.addCopy.post(requestBody);
}


```