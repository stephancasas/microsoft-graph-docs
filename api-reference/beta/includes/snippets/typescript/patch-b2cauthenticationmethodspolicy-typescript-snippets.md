---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new B2cAuthenticationMethodsPolicy();
requestBody.isEmailPasswordAuthenticationEnabled = false;
requestBody.isUserNameAuthenticationEnabled = true;
requestBody.isPhoneOneTimePasswordAuthenticationEnabled = true;
const result = async () => {
	await graphServiceClient.policies.b2cAuthenticationMethodsPolicy.patch(requestBody);
}


```