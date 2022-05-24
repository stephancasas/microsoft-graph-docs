---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter%20 : "%20principalIds/any",
};
const result = async () => {
	await graphServiceClient.roleManagement.deviceManagement.roleAssignments.get(requestParameters);
}


```