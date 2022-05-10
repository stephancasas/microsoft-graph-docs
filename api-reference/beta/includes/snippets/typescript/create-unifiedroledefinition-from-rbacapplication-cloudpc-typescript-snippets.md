---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleDefinition();
requestBody.description = "An example custom role";
requestBody.displayName = "ExampleCustomRole";
const unifiedrolepermission = new UnifiedRolePermission();
unifiedrolepermission.additionalData = {
					 "allowedResourceActions" : [
							"Microsoft.CloudPC/CloudPCs/Read"
						]
				 }
requestBody.rolePermissions = [
			unifiedrolepermission
		]
requestBody.additionalData = {
		 "condition" : "null"
	 }
const result = async () => {
	await graphServiceClient.roleManagement.cloudPC.roleDefinitions.post(requestBody);
}


```