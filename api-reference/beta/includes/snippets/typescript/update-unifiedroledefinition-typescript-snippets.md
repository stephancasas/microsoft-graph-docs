---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleDefinition();
requestBody.description = "Update basic properties of application registrations";
requestBody.displayName = "Application Registration Support Administrator";
const unifiedrolepermission = new UnifiedRolePermission();
unifiedrolepermission.additionalData = {
					 "allowedResourceActions" : [
							"microsoft.directory/applications/basic/read"
						]
				 }
requestBody.rolePermissions = [
			unifiedrolepermission
		]
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleDefinitionsById("unifiedRoleDefinition-id").patch(requestBody);
}


```