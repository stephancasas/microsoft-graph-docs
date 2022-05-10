---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "Here's the latest budget. <attachment id="153fa47d-18c9-4179-be08-9879815a9f90"></attachment>";
const chatmessageattachment = new ChatMessageAttachment();
chatmessageattachment.additionalData = {
					 "id" : "153fa47d-18c9-4179-be08-9879815a9f90",
					 "contentType" : "reference",
					 "contentUrl" : "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
					 "name" : "Budget.docx"
				 }
requestBody.attachments = [
			chatmessageattachment
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```