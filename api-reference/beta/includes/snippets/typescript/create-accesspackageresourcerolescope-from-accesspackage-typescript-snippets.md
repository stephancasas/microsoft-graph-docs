---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRoleScope();
requestBody.accessPackageResourceRole = new AccessPackageResourceRole();
requestBody.accessPackageResourceRole.originId = "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca";
requestBody.accessPackageResourceRole.displayName = "Member";
requestBody.accessPackageResourceRole.originSystem = "AadGroup";
requestBody.accessPackageResourceRole.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResourceRole.accessPackageResource.id = "1d08498d-72a1-403f-8511-6b1f875746a0";
requestBody.accessPackageResourceRole.accessPackageResource.resourceType = "O365 Group";
requestBody.accessPackageResourceRole.accessPackageResource.originId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca";
requestBody.accessPackageResourceRole.accessPackageResource.originSystem = "AadGroup";
requestBody.accessPackageResourceScope = new AccessPackageResourceScope();
requestBody.accessPackageResourceScope.originId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca";
requestBody.accessPackageResourceScope.originSystem = "AadGroup";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackagesById("accessPackage-id").accessPackageResourceRoleScopes.post(requestBody);
}


```