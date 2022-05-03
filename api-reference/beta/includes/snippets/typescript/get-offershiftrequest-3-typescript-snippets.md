---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OfferShiftRequest();
requestBody.senderShiftId = "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29";
requestBody.senderMessage = "Having a family emergency, could you take this shift for me?";
requestBody.recipientUserId = "fe278b61-21ac-4872-8b41-1962bbb98e3c";
const headers = {
	"Authorization": "Bearer {token}",
};
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.offerShiftRequests.post(requestBody, headers);
}


```