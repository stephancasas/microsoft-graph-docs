---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	id : "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D",
};
async () => {
	await graphServiceClient.groupsById("group-id").rejectedSenders.$ref.delete(requestParameters);
}


```