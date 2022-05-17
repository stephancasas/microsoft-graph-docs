---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "VideoTeleconferenceId%20eq%20'123456789'",
};
const result = async () => {
	await graphServiceClient.communications.onlineMeetings.get(requestParameters);
}


```