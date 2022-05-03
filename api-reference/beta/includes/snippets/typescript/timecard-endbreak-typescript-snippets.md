---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EndbreakRequestBody();
requestBody.notes = new ItemBody();
requestBody.notes.contentType = BodyType.Text;
requestBody.notes.content = "end break smaple notes";
requestBody.additionalData = {
		 "atAprovedLocation" : true
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCardsById("timeCard-id").endBreak.post(requestBody);
}


```