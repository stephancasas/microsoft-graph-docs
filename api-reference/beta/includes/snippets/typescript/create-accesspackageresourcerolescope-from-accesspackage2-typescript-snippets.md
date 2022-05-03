---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRoleScope();
requestBody.accessPackageResourceRole = new AccessPackageResourceRole();
requestBody.accessPackageResourceRole.originId = "4";
requestBody.accessPackageResourceRole.originSystem = "SharePointOnline";
requestBody.accessPackageResourceRole.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResourceRole.accessPackageResource.id = "53c71803-a0a8-4777-aecc-075de8ee3991";
requestBody.accessPackageResourceScope = new AccessPackageResourceScope();
requestBody.accessPackageResourceScope.id = "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33";
requestBody.accessPackageResourceScope.originId = "https://microsoft.sharepoint.com/portals/Community";
requestBody.accessPackageResourceScope.originSystem = "SharePointOnline";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackagesById("accessPackage-id").accessPackageResourceRoleScopes.post(requestBody);
}


```