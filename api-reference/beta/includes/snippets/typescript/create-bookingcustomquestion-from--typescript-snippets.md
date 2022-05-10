---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new 3bc6fde0-4ad3-445d-ab17-0fc15dba0774RequestBody();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.bookingCustomQuestion",
		 "displayName" : "What is your age?",
		 "answerInputType" : "text",
		 "answerOptions" : [
			]
	 }
async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").customQuestionsById("bookingCustomQuestion-id").post(requestBody);
}


```