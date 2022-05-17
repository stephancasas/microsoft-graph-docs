---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "Extensions/any",
	expand : "Extensions($filter=id%20eq%20'Com.Contoso.Referral')",
};
const result = async () => {
	await graphServiceClient.me.messages.get(requestParameters);
}


```