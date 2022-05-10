---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "MentionsPreview/IsMentioned%20eq%20true",
	select : "Subject,Sender,ReceivedDateTime,MentionsPreview",
};
const result = async () => {
	await graphServiceClient.me.messages.get(requestParameters);
}


```