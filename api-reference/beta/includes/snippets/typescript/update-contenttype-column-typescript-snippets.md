---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ColumnDefinition();
requestBody.required = true;
requestBody.hidden = false;
requestBody.propagateChanges = false;
const result = async () => {
	await graphServiceClient.sitesById("site-id").contentTypesById("contentType-id").columnsById("columnDefinition-id").patch(requestBody);
}


```