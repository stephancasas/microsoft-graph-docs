---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessReviewReviewer();
requestBody.id = "006111db-0810-4494-a6df-904d368bd81b";
const result = async () => {
	await graphServiceClient.accessReviewsById("accessReview-id").reviewers.post(requestBody);
}


```