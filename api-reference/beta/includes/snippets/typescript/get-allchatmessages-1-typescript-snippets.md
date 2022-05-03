---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	top : 2,
	orderBy : "createdDateTime%20desc",
};
const result = async () => {
	await graphServiceClient.chatsById("chat-id").messages.get(requestParameters);
}


```