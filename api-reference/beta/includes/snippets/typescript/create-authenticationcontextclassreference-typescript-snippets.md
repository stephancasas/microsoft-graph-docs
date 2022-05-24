---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthenticationContextClassReference();
requestBody.id = "c1";
requestBody.displayName = "Contoso medium";
requestBody.description = "Medium protection level defined for Contoso policy";
requestBody.isAvailable = true;
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.authenticationContextClassReferences.post(requestBody);
}


```