---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "inheritsPermissionsFrom",
};
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleDefinitionsById("unifiedRoleDefinition-id").get(requestParameters);
}


```