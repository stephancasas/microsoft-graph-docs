---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CopyToDefaultContentLocationRequestBody();
requestBody.sourceFile = new ItemReference();
requestBody.sourceFile.sharepointIds = new SharepointIds();
requestBody.sourceFile.sharepointIds.listId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0";
requestBody.sourceFile.sharepointIds.listItemId = "2";
requestBody.destinationFileName = "newname.txt";
async () => {
	await graphServiceClient.sitesById("site-id").contentTypesById("contentType-id").copyToDefaultContentLocation.post(requestBody);
}


```