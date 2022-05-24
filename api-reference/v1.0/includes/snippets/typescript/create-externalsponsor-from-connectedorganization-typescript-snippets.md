---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/v1.0/users/{id}"
	 }
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizationsById("connectedOrganization-id").externalSponsors.$ref.post(requestBody);
}


```