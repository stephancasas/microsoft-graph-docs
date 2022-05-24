---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ContinuousAccessEvaluationPolicy();
requestBody.migrate = true;
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.continuousAccessEvaluationPolicy"
	 }
const result = async () => {
	await graphServiceClient.identity.continuousAccessEvaluationPolicy.patch(requestBody);
}


```