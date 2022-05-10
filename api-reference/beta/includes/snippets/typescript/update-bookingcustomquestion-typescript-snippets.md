---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BookingCustomQuestion();
requestBody.displayName = "What is your age?";
requestBody.answerInputType = AnswerInputType.Text;
requestBody.answerOptions = [
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.bookingCustomQuestion"
	 }
const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").customQuestionsById("bookingCustomQuestion-id").patch(requestBody);
}


```