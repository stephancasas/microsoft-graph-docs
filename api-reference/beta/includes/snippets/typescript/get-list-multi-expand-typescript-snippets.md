---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	select : "name,lastModifiedDateTime",
	expand : "columns(select=name,description),items)",
};
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").get(requestParameters);
}


```