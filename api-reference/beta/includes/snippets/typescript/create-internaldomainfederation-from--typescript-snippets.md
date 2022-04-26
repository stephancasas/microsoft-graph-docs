---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new InternalDomainFederation();
requestBody.displayName = "Contoso";
requestBody.issuerUri = "http://contoso.com/adfs/services/trust";
requestBody.metadataExchangeUri = "https://sts.contoso.com/adfs/services/trust/mex";
requestBody.signingCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI";
requestBody.passiveSignInUri = "https://sts.contoso.com/adfs/ls";
requestBody.preferredAuthenticationProtocol = AuthenticationProtocol.WsFed;
requestBody.activeSignInUri = "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed";
requestBody.signOutUri = "https://sts.contoso.com/adfs/ls";
requestBody.promptLoginBehavior = PromptLoginBehavior.NativeSupport;
requestBody.isSignedAuthenticationRequestRequired = true;
requestBody.nextSigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI";
requestBody.federatedIdpMfaBehavior = FederatedIdpMfaBehavior.RejectMfaByFederatedIdp;
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.internalDomainFederation"
	 }
const result = async () => {
	await graphServiceClient.domainsById("domain-id").federationConfiguration.post(requestBody);
}


```