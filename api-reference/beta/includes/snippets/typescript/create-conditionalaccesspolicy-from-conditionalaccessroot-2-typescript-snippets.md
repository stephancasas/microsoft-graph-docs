---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConditionalAccessPolicy();
requestBody.displayName = "Block access to EXO non-trusted regions.";
requestBody.state = ConditionalAccessPolicyState.Enabled;
requestBody.conditions = new ConditionalAccessConditionSet();
requestBody.conditions.clientAppTypes = [
				"all"
			]
requestBody.conditions.applications = new ConditionalAccessApplications();
requestBody.conditions.applications.includeApplications = [
					"00000002-0000-0ff1-ce00-000000000000"
				]
requestBody.conditions.users = new ConditionalAccessUsers();
requestBody.conditions.users.includeGroups = [
					"ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
				]
requestBody.conditions.locations = new ConditionalAccessLocations();
requestBody.conditions.locations.includeLocations = [
					"198ad66e-87b3-4157-85a3-8a7b51794ee9"
				]
requestBody.grantControls = new ConditionalAccessGrantControls();
requestBody.grantControls.operator = "OR";
requestBody.grantControls.builtInControls = [
				"block"
			]
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.post(requestBody);
}


```