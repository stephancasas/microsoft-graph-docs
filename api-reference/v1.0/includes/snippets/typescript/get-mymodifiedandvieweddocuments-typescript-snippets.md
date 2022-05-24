---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	orderby : "LastUsed/LastAccessedDateTime%20desc",
};
const result = async () => {
	await graphServiceClient.me.insights.used.get(requestParameters);
}


```