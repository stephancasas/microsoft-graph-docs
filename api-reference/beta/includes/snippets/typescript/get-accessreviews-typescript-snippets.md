---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "businessFlowTemplateId%20eq%20'6e4f3d20-c5c3-407f-9695-8460952bcc68'",
	top : 100,
	skip : 0,
};
const result = async () => {
	await graphServiceClient.accessReviews.get(requestParameters);
}


```