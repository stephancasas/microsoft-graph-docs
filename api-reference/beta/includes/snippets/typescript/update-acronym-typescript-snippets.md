---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Acronym();
requestBody.description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.";
const result = async () => {
	await graphServiceClient.search.acronymsById("acronym-id").patch(requestBody);
}


```