---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ScopedRoleMembership();
requestBody.roleId = "roleId-value";
requestBody.roleMemberInfo = new Identity();
requestBody.roleMemberInfo.id = "id-value";
const result = async () => {
	await graphServiceClient.directory.administrativeUnitsById("administrativeUnit-id").scopedRoleMembers.post(requestBody);
}


```