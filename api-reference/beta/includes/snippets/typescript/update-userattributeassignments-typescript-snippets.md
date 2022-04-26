---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityUserFlowAttributeAssignment();
requestBody.userInputType = IdentityUserFlowAttributeInputType.TextBox;
const result = async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").userAttributeAssignmentsById("identityUserFlowAttributeAssignment-id").patch(requestBody);
}


```