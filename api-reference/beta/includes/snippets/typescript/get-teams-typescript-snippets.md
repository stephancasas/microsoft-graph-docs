---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "displayName%20eq%20'A%20Contoso%20Team'",
	select : "id,description",
};
const result = async () => {
	await graphServiceClient.teams.get(requestParameters);
}


```