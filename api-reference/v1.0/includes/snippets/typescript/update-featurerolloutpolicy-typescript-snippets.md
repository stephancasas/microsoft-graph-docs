---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new FeatureRolloutPolicy();
requestBody.displayName = "PasswordHashSync Rollout Policy";
requestBody.description = "PasswordHashSync Rollout Policy";
requestBody.isEnabled = true;
requestBody.isAppliedToOrganization = false;
const result = async () => {
	await graphServiceClient.policies.featureRolloutPoliciesById("featureRolloutPolicy-id").patch(requestBody);
}


```