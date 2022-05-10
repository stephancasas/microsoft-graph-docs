---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConditionalAccessPolicy();
requestBody.displayName = "Require MFA to EXO from non-compliant devices.";
requestBody.state = ConditionalAccessPolicyState.Enabled;
requestBody.conditions = new ConditionalAccessConditionSet();
requestBody.conditions.applications = new ConditionalAccessApplications();
requestBody.conditions.applications.includeApplications = [
					"00000002-0000-0ff1-ce00-000000000000"
				]
requestBody.conditions.users = new ConditionalAccessUsers();
requestBody.conditions.users.includeGroups = [
					"ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
				]
requestBody.grantControls = new ConditionalAccessGrantControls();
requestBody.grantControls.operator = "OR";
requestBody.grantControls.builtInControls = [
				"mfa"
			]
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.post(requestBody);
}


```