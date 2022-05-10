---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TokenIssuancePolicy();
requestBody.definition = [
			"definition-value"
		]
requestBody.displayName = "displayName-value";
requestBody.isOrganizationDefault = true;
const result = async () => {
	await graphServiceClient.policies.tokenIssuancePolicies.post(requestBody);
}


```