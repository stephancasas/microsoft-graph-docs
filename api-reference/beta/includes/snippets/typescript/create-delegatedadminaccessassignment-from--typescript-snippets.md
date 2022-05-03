---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DelegatedAdminAccessAssignment();
requestBody.accessContainer = new DelegatedAdminAccessContainer();
requestBody.accessContainer.accessContainerId = "869713c9-0b28-4d08-8949-ae07ae1bf528";
requestBody.accessContainer.accessContainerType = DelegatedAdminAccessContainerType.SecurityGroup;
requestBody.accessDetails = new DelegatedAdminAccessDetails();
const unifiedrole = new UnifiedRole();
unifiedrole.additionalData = {
						 "roleDefinitionId" : "29232cdf-9323-42fd-ade2-1d097af3e4de"
					 }
const unifiedrole1 = new UnifiedRole();
unifiedrole1.additionalData = {
						 "roleDefinitionId" : "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
					 }
const unifiedrole2 = new UnifiedRole();
unifiedrole2.additionalData = {
						 "roleDefinitionId" : "729827e3-9c14-49f7-bb1b-9608f156bbb8"
					 }
const unifiedrole3 = new UnifiedRole();
unifiedrole3.additionalData = {
						 "roleDefinitionId" : "3a2c62db-5318-420d-8d74-23affee5d9d5"
					 }
requestBody.accessDetails.unifiedRoles = [
				unifiedrole,
				unifiedrole1,
				unifiedrole2,
				unifiedrole3
			]
const result = async () => {
	await graphServiceClient.tenantRelationships.delegatedAdminRelationshipsById("delegatedAdminRelationship-id").accessAssignments.post(requestBody);
}


```