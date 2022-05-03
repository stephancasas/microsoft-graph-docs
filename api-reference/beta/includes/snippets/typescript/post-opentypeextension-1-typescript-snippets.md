---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.subject = "Annual review";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.HTML;
requestBody.body.content = "You should be proud!";
const recipient = new Recipient();
recipient.additionalData = {
						 ["address" , "rufus@contoso.com"],
				 }
requestBody.toRecipients = [
			recipient
		]
const extension = new Extension();
extension.additionalData = {
					 "@odata.type" : "microsoft.graph.openTypeExtension",
					 "extensionName" : "Com.Contoso.Referral",
					 "companyName" : "Wingtip Toys",
					 "expirationDate" : "2015-12-30T11:00:00.000Z",
					 "dealValue" : 10000
				 }
requestBody.extensions = [
			extension
		]
const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```