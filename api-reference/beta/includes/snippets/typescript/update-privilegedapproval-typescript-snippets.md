---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrivilegedApproval();
requestBody.approvalState = ApprovalState.ApprovalState-value;
requestBody.approverReason = "approverReason-value";
const result = async () => {
	await graphServiceClient.privilegedApprovalById("privilegedApproval-id").patch(requestBody);
}


```