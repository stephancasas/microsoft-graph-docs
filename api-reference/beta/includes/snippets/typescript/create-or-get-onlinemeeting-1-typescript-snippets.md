---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateOrGetRequestBody();
requestBody.startDateTime =  new Date("2020-02-06T01:49:21.3524945+00:00");
requestBody.endDateTime =  new Date("2020-02-06T02:19:21.3524945+00:00");
requestBody.subject = "Create a meeting with customId provided";
requestBody.externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";
requestBody.participants = new MeetingParticipants();
const meetingparticipantinfo = new MeetingParticipantInfo();
meetingparticipantinfo.additionalData = {
								 ["id" , "1f35f2e6-9cab-44ad-8d5a-b74c14720000"],
						 "role" : "presenter",
						 "upn" : "test1@contoso.com"
					 }
requestBody.participants.attendees = [
				meetingparticipantinfo
			]
const result = async () => {
	await graphServiceClient.me.onlineMeetings.createOrGet.post(requestBody);
}


```