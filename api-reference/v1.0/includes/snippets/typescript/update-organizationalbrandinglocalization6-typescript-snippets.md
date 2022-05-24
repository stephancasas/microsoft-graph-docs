---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OrganizationalBrandingLocalization();
requestBody.backgroundColor = "#00000F";
requestBody.signInPageText = "Welcome to Contoso France";
const result = async () => {
	await graphServiceClient.organizationById("organization-id").branding.localizationsById("organizationalBrandingLocalization-id").patch(requestBody);
}


```