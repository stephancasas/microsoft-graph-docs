---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	forcedelete : true,
};
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").tagsById("tag-id").delete(requestParameters);
}


```