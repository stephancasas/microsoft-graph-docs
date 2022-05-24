---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	select : "*,parentSiteId",
};
const result = async () => {
	await graphServiceClient.sitesById("site-id").termStore.groupsById("group-id").get(requestParameters);
}


```