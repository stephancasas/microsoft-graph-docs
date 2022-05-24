---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const headers = {
	"ConsistencyLevel": "eventual",
};
let requestParameters = {
	count : true,
	filter : "principalId%20eq%20'2c7936bc-3517-40f3-8eda-4806637b6516'%20and%20directoryScopeId%20eq%20'/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'",
};
const result = async () => {
	await graphServiceClient.roleManagement.directory.transitiveRoleAssignments.get(requestParameters, headers);
}


```