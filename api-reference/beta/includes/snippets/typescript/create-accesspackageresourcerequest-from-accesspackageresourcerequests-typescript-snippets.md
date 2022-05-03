---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRequest();
requestBody.catalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5";
requestBody.requestType = "AdminAdd";
requestBody.justification = "";
requestBody.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResource.displayName = "Sales";
requestBody.accessPackageResource.description = "https://contoso.sharepoint.com/sites/Sales";
requestBody.accessPackageResource.url = "https://contoso.sharepoint.com/sites/Sales";
requestBody.accessPackageResource.resourceType = "SharePoint Online Site";
requestBody.accessPackageResource.originId = "https://contoso.sharepoint.com/sites/Sales";
requestBody.accessPackageResource.originSystem = "SharePointOnline";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```