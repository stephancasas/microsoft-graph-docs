---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new User();
requestBody.displayName = "John Smith";
const objectidentity = new ObjectIdentity();
objectidentity.additionalData = {
					 "signInType" : "userName",
					 "issuer" : "contoso.onmicrosoft.com",
					 "issuerAssignedId" : "johnsmith"
				 }
const objectidentity1 = new ObjectIdentity();
objectidentity1.additionalData = {
					 "signInType" : "emailAddress",
					 "issuer" : "contoso.onmicrosoft.com",
					 "issuerAssignedId" : "jsmith@yahoo.com"
				 }
const objectidentity2 = new ObjectIdentity();
objectidentity2.additionalData = {
					 "signInType" : "federated",
					 "issuer" : "facebook.com",
					 "issuerAssignedId" : "5eecb0cd"
				 }
requestBody.identities = [
			objectidentity,
			objectidentity1,
			objectidentity2
		]
requestBody.passwordProfile = new PasswordProfile();
requestBody.passwordProfile.password = "password-value";
requestBody.passwordProfile.forceChangePasswordNextSignIn = false;
requestBody.passwordPolicies = "DisablePasswordExpiration";
const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```