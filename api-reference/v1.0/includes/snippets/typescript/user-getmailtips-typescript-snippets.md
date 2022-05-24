---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetMailTipsRequestBody();
requestBody.emailAddresses = [
			"danas@contoso.onmicrosoft.com",
			"fannyd@contoso.onmicrosoft.com"
		]
requestBody.mailTipsOptions = MailTipsType.AutomaticReplies, mailboxFullStatus;
const result = async () => {
	await graphServiceClient.me.getMailTips.post(requestBody);
}


```