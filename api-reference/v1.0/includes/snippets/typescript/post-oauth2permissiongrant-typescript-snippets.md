---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OAuth2PermissionGrant();
requestBody.clientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5";
requestBody.consentType = "AllPrincipals";
requestBody.resourceId = "943603e4-e787-4fe9-93d1-e30f749aae39";
requestBody.scope = "DelegatedPermissionGrant.ReadWrite.All";
const result = async () => {
	await graphServiceClient.oauth2PermissionGrants.post(requestBody);
}


```