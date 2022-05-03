---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new 3ddfcfc8-9383-446f-83cc-3ab9be4be18fRequestBody();
requestBody.additionalData = {
		 "emailAddress" : "kim@contoso.com"
	 }
async () => {
	await graphServiceClient.usersById("user-id").authentication.emailMethodsById("emailAuthenticationMethod-id").put(requestBody);
}


```