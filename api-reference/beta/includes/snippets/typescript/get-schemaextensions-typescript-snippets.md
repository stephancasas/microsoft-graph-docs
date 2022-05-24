---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "id%20eq%20'graphlearn_test'",
};
const result = async () => {
	await graphServiceClient.schemaExtensions.get(requestParameters);
}


```