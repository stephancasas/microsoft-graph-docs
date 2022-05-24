---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.subject = null,
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "<attachment id="74d20c7f34aa4a7fb74e2b30004247c5"></attachment>";
const chatmessageattachment = new ChatMessageAttachment();
chatmessageattachment.additionalData = {
					 "id" : "74d20c7f34aa4a7fb74e2b30004247c5",
					 "contentType" : "application/vnd.microsoft.card.thumbnail",
					 "contentUrl" : null,
					 "content" : "{
  "title": "This is an example of posting a card",
  "subtitle": "<h3>This is the subtitle</h3>",
  "text": "Here is some body text. <br>\r\nAnd a <a href=\"http://microsoft.com/\">hyperlink</a>. <br>\r\nAnd below that is some buttons:",
  "buttons": [
    {
      "type": "messageBack",
      "title": "Login to FakeBot",
      "text": "login",
      "displayText": "login",
      "value": "login"
    }
  ]
}",
					 "name" : null,
					 "thumbnailUrl" : null,
					 "teamsAppId" : "881b8843-fd91-49e5-9ac2-47ec497ffbe5"
				 }
requestBody.attachments = [
			chatmessageattachment
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```