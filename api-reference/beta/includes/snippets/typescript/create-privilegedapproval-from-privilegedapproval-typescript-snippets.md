---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrivilegedApproval();
requestBody.userId = "userId-value";
requestBody.roleId = "roleId-value";
requestBody.approvalType = "approvalType-value";
requestBody.approvalState = ApprovalState.ApprovalState-value;
requestBody.approvalDuration = "datetime-value";
const result = async () => {
	await graphServiceClient.privilegedApproval.post(requestBody);
}


```