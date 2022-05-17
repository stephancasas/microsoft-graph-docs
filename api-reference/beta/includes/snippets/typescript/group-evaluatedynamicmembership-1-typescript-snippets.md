---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EvaluateDynamicMembershipRequestBody();
requestBody.memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";
const result = async () => {
	await graphServiceClient.groupsById("group-id").evaluateDynamicMembership.post(requestBody);
}


```