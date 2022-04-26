---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdatePasswordSingleSignOnCredentialsRequestBody();
requestBody.id = "5793aa3b-cca9-4794-679a240f8b58";
const credential = new Credential();
credential.additionalData = {
					 "fieldId" : "param_username",
					 "value" : "myusername",
					 "type" : "username"
				 }
const credential1 = new Credential();
credential1.additionalData = {
					 "fieldId" : "param_password",
					 "value" : "pa$$w0rd",
					 "type" : "password"
				 }
requestBody.credentials = [
			credential,
			credential1
		]
async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").updatePasswordSingleSignOnCredentials.post(requestBody);
}


```