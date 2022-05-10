---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityUserFlowAttributeAssignment();
requestBody.isOptional = false;
requestBody.requiresVerification = false;
requestBody.userInputType = IdentityUserFlowAttributeInputType.TextBox;
requestBody.displayName = "Shoe size";
requestBody.userAttributeValues = [
		]
requestBody.userAttribute = new IdentityUserFlowAttribute();
requestBody.userAttribute.id = "extension_guid_shoeSize";
const result = async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").userAttributeAssignments.post(requestBody);
}


```