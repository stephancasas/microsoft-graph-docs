---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')",
};
const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.get(requestParameters);
}


```