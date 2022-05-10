---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new MeetingRegistrationQuestion();
requestBody.answerInputType = AnswerInputType.RadioButton;
requestBody.answerOptions = [
			"Software Engineer",
			"Software Development Manager",
			"Product Manager",
			"Data scientist",
			"Other"
		]
const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.customQuestionsById("meetingRegistrationQuestion-id").patch(requestBody);
}


```