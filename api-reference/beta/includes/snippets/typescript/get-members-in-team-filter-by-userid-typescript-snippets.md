---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "(microsoft.graph.aadUserConversationMember/userId%20eq%20'73761f06-2ac9-469c-9f10-279a8cc267f9')",
};
const result = async () => {
	await graphServiceClient.teamsById("team-id").members.get(requestParameters);
}


```