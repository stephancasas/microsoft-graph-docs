---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "membershipType%20eq%20'shared'",
};
const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.get(requestParameters);
}


```