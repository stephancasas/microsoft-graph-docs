---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TimeCard();
requestBody.clockInEvent = new TimeCardEvent();
requestBody.clockInEvent.dateTime =  new Date("2019-03-18T00:00:00.000Z");
requestBody.clockInEvent.atApprovedLocation = true;
requestBody.clockInEvent.notes = new ItemBody();
requestBody.clockInEvent.notes.content = "Started late due to traffic in CA 237";
requestBody.clockInEvent.notes.contentType = BodyType.Text;
requestBody.notes = new ItemBody();
requestBody.notes.content = "8 To 5 Inventory management";
requestBody.notes.contentType = BodyType.Text;
const timecardbreak = new TimeCardBreak();
timecardbreak.additionalData = {
					 "breakId" : "string",
						 ["content" , "Lunch break"],
						 ["contentType" , "text"],
						 ["dateTime" , "2019-03-18T02:00:00.000Z"],
						 ["atApprovedLocation" , true],
							 ["content" , "Reduced break to make up for lost time"],
							 ["contentType" , "text"],
				 }
requestBody.breaks = [
			timecardbreak
		]
requestBody.additionalData = {
		 "onBehalfOfUserId" : "a3601044-a1b5-438e-b742-f78d01d68a67"
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCards.post(requestBody);
}


```