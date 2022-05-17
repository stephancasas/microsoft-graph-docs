---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DelegatedAdminRelationshipRequest();
requestBody.action = DelegatedAdminRelationshipRequestAction.LockForApproval;
const result = async () => {
	await graphServiceClient.tenantRelationships.delegatedAdminRelationshipsById("delegatedAdminRelationship-id").requests.post(requestBody);
}


```