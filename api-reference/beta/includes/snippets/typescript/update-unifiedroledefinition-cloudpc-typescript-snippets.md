---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleDefinition();
requestBody.description = "Update basic properties and permission of application registrations";
requestBody.displayName = "ExampleCustomRole";
const unifiedrolepermission = new UnifiedRolePermission();
unifiedrolepermission.additionalData = {
					 "allowedResourceActions" : [
							"Microsoft.CloudPC/CloudPCs/Read",
							"Microsoft.CloudPC/CloudPCs/Reprovision"
						]
				 }
requestBody.rolePermissions = [
			unifiedrolepermission
		]
const result = async () => {
	await graphServiceClient.roleManagement.cloudPC.roleDefinitionsById("unifiedRoleDefinition-id").patch(requestBody);
}


```