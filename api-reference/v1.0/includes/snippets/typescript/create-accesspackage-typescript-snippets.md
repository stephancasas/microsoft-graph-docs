---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackage();
requestBody.displayName = "sales reps";
requestBody.description = "outside sales representatives";
requestBody.isHidden = false;
requestBody.catalog = new AccessPackageCatalog();
requestBody.catalog.id = "66584aae-98bb-48cc-9458-7bee5d2a6577";
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackages.post(requestBody);
}


```