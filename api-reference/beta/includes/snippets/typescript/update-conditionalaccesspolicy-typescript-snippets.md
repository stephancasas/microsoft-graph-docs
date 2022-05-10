---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConditionalAccessPolicy();
requestBody.conditions = new ConditionalAccessConditionSet();
requestBody.conditions.signInRiskLevels = [
				"high",
				"medium",
				"low"
			]
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policiesById("conditionalAccessPolicy-id").patch(requestBody);
}


```