---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OrganizationalBranding();
requestBody.signInPageText = "Default";
requestBody.usernameHintText = "DefaultHint";
const headers = {
	"Accept-Language": "0",
};
const result = async () => {
	await graphServiceClient.organizationById("organization-id").branding.patch(requestBody, headers);
}


```