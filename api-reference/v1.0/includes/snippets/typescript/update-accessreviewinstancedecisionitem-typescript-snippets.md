---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessReviewInstanceDecisionItem();
requestBody.decision = "Approve";
requestBody.justification = "Kathleen still needs access to the Marketing group as she works in the Marketing organization.";
const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").instancesById("accessReviewInstance-id").decisionsById("accessReviewInstanceDecisionItem-id").patch(requestBody);
}


```