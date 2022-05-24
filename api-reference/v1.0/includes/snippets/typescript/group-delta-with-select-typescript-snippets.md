---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	select : "displayName,description,mailNickname",
};
const result = async () => {
	await graphServiceClient.groups.delta().get(requestParameters);
}


```