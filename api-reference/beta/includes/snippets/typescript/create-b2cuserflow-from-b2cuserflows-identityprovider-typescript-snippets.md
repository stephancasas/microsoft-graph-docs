---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new B2cIdentityUserFlow();
requestBody.id = "Customer";
requestBody.userFlowType = UserFlowType.SignUpOrSignIn;
requestBody.userFlowTypeVersion = 3;
const identityprovider = new IdentityProvider();
identityprovider.additionalData = {
					 "id" : "Facebook-OAuth"
				 }
requestBody.identityProviders = [
			identityprovider
		]
const headers = {
	"Location": "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')",
};
const result = async () => {
	await graphServiceClient.identity.b2cUserFlows.post(requestBody, headers);
}


```