---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConnectedOrganization();
requestBody.displayName = "Connected organization name";
requestBody.description = "Connected organization description";
const identitysource = new IdentitySource();
identitysource.additionalData = {
					 "@odata.type" : "#microsoft.graph.domainIdentitySource",
					 "domainName" : "example.com",
					 "displayName" : "example.com"
				 }
requestBody.identitySources = [
			identitysource
		]
requestBody.state = ConnectedOrganizationState.Proposed;
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizations.post(requestBody);
}


```