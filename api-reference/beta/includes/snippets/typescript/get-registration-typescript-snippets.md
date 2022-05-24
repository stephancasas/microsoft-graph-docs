---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "microsoft.graph.meetingRegistration/customQuestions",
};
const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.get(requestParameters);
}


```