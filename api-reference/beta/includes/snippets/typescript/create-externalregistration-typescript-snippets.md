---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new RegistrationRequestBody();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.externalMeetingRegistration",
		 "allowedRegistrant" : "everyone"
	 }
async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").registration.post(requestBody);
}


```