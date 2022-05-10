---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRequest();
requestBody.catalogId = "de9315c1-272b-4905-924b-cc112ca180c7";
requestBody.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResource.displayName = "Community Outreach";
requestBody.accessPackageResource.description = "https://contoso.sharepoint.com/sites/CSR";
requestBody.accessPackageResource.resourceType = "SharePoint Online Site";
requestBody.accessPackageResource.originId = "https://contoso.sharepoint.com/sites/CSR";
requestBody.accessPackageResource.originSystem = "SharePointOnline";
requestBody.accessPackageResource.accessPackageResourceEnvironment = new AccessPackageResourceEnvironment();
requestBody.accessPackageResource.accessPackageResourceEnvironment.originId = "https://contoso-admin.sharepoint.com/";
requestBody.requestType = "AdminAdd";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```