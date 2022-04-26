---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityProvider();
requestBody.name = "Login with the Contoso identity provider";
requestBody.type = "OpenIDConnect";
requestBody.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
requestBody.clientSecret = "12345";
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.openIdConnectProvider",
			 ["userId" , "myUserId"],
			 ["givenName" , "myGivenName"],
			 ["surname" , "mySurname"],
			 ["email" , "myEmail"],
			 ["displayName" , "myDisplayName"],
		 "domainHint" : "mycustomoidc",
		 "metadataUrl" : "https://mycustomoidc.com/.well-known/openid-configuration",
		 "responseMode" : "form_post",
		 "responseType" : "code",
		 "scope" : "openid"
	 }
const result = async () => {
	await graphServiceClient.identityProviders.post(requestBody);
}


```