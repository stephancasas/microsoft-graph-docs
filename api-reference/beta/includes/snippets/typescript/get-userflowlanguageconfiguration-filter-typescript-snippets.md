---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "isEnabled%20eq%20true",
};
const result = async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").languages.get(requestParameters);
}


```