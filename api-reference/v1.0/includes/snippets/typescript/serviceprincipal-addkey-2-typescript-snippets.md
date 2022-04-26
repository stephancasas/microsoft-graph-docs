---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddKeyRequestBody();
requestBody.keyCredential = new KeyCredential();
requestBody.keyCredential.type = "X509CertAndPassword";
requestBody.keyCredential.usage = "Sign";
requestBody.keyCredential.key = btoa("MIIDYDCCAki...");
requestBody.passwordCredential = new PasswordCredential();
requestBody.passwordCredential.secretText = "MKTr0w1...";
requestBody.proof = "eyJ0eXAiOiJ...";
const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").addKey.post(requestBody);
}


```