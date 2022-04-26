---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "roleDefinitionId%20eq%20'62e90394-69f5-4237-9190-012177145e10'",
	expand : "principal",
};
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.get(requestParameters);
}


```