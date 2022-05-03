---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DelegatedAdminAccessAssignment();
requestBody.accessDetails = new DelegatedAdminAccessDetails();
const unifiedrole = new UnifiedRole();
unifiedrole.additionalData = {
						 "roleDefinitionId" : "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
					 }
const unifiedrole1 = new UnifiedRole();
unifiedrole1.additionalData = {
						 "roleDefinitionId" : "44367163-eba1-44c3-98af-f5787879f96a"
					 }
const unifiedrole2 = new UnifiedRole();
unifiedrole2.additionalData = {
						 "roleDefinitionId" : "729827e3-9c14-49f7-bb1b-9608f156bbb8"
					 }
requestBody.accessDetails.unifiedRoles = [
				unifiedrole,
				unifiedrole1,
				unifiedrole2
			]
const headers = {
	"If-Match": "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
};
const result = async () => {
	await graphServiceClient.tenantRelationships.delegatedAdminRelationshipsById("delegatedAdminRelationship-id").accessAssignmentsById("delegatedAdminAccessAssignment-id").patch(requestBody, headers);
}


```