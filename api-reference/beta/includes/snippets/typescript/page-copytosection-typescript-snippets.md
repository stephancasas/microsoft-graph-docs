---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CopyToSectionRequestBody();
requestBody.id = "id-value";
requestBody.groupId = "groupId-value";
const result = async () => {
	await graphServiceClient.me.onenote.pagesById("onenotePage-id").copyToSection.post(requestBody);
}


```