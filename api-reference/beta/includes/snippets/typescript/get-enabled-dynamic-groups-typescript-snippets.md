---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT)%20and%20membershipRuleProcessingState%20eq%20'On'",
	count : true,
	select : "id,membershipRule,membershipRuleProcessingState",
};
const result = async () => {
	await graphServiceClient.groups.get(requestParameters);
}


```