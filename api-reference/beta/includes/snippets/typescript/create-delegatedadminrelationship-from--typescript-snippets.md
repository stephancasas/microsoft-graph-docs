---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DelegatedAdminRelationship();
requestBody.displayName = "Contoso admin relationship";
requestBody.duration = "P730D";
requestBody.customer = new DelegatedAdminRelationshipCustomerParticipant();
requestBody.customer.tenantId = "4b827261-d21f-4aa9-b7db-7fa1f56fb163";
requestBody.customer.displayName = "Contoso subsidiary Inc";
requestBody.accessDetails = new DelegatedAdminAccessDetails();
const unifiedrole = new UnifiedRole();
unifiedrole.additionalData = {
						 "roleDefinitionId" : "29232cdf-9323-42fd-ade2-1d097af3e4de"
					 }
const unifiedrole1 = new UnifiedRole();
unifiedrole1.additionalData = {
						 "roleDefinitionId" : "3a2c62db-5318-420d-8d74-23affee5d9d5"
					 }
requestBody.accessDetails.unifiedRoles = [
				unifiedrole,
				unifiedrole1
			]
const result = async () => {
	await graphServiceClient.tenantRelationships.delegatedAdminRelationships.post(requestBody);
}


```