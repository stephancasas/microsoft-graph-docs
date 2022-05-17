---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SetOrderRequestBody();
requestBody.newAssignmentOrder = new AssignmentOrder();
requestBody.newAssignmentOrder.order = [
				"City",
				"extension_GUID_ShoeSize"
			]
async () => {
	await graphServiceClient.identity.b2xUserFlowsById("b2xIdentityUserFlow-id").userAttributeAssignments.setOrder.post(requestBody);
}


```