---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter%20 : "%20principalId%20eq%20'f1847572-48aa-47aa-96a3-2ec61904f41f'",
};
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.get(requestParameters);
}


```