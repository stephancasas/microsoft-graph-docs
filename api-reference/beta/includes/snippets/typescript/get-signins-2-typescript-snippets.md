---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "startsWith(appDisplayName,'Azure')",
	top : 10,
};
const result = async () => {
	await graphServiceClient.auditLogs.signIns.get(requestParameters);
}


```