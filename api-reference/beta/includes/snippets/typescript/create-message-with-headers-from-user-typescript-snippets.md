---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.subject = "9/8/2018: concert";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.HTML;
requestBody.body.content = "The group represents Washington.";
const recipient = new Recipient();
recipient.additionalData = {
						 ["address" , "AlexW@contoso.OnMicrosoft.com"],
				 }
requestBody.toRecipients = [
			recipient
		]
const internetmessageheader = new InternetMessageHeader();
internetmessageheader.additionalData = {
					 "name" : "x-custom-header-group-name",
					 "value" : "Washington"
				 }
const internetmessageheader1 = new InternetMessageHeader();
internetmessageheader1.additionalData = {
					 "name" : "x-custom-header-group-id",
					 "value" : "WA001"
				 }
requestBody.internetMessageHeaders = [
			internetmessageheader,
			internetmessageheader1
		]
const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```