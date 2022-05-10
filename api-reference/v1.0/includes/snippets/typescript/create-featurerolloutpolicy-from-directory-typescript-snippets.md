---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new FeatureRolloutPolicy();
requestBody.displayName = "PassthroughAuthentication rollout policy";
requestBody.description = "PassthroughAuthentication rollout policy";
requestBody.feature = StagedFeatureName.PassthroughAuthentication;
requestBody.isEnabled = true;
requestBody.isAppliedToOrganization = false;
const result = async () => {
	await graphServiceClient.policies.featureRolloutPolicies.post(requestBody);
}


```