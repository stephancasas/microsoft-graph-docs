---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new InternalDomainFederation();
requestBody.displayName = "Contoso name change";
requestBody.federatedIdpMfaBehavior = FederatedIdpMfaBehavior.AcceptIfMfaDoneByFederatedIdp;
const result = async () => {
	await graphServiceClient.domainsById("domain-id").federationConfigurationById("internalDomainFederation-id").patch(requestBody);
}


```