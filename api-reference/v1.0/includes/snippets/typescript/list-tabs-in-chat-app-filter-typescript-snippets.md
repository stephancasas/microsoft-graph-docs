---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "teamsApp",
	filter : "teamsApp/id%20eq%20'com.microsoft.teamspace.tab.web'",
};
const result = async () => {
	await graphServiceClient.chatsById("chat-id").tabs.get(requestParameters);
}


```