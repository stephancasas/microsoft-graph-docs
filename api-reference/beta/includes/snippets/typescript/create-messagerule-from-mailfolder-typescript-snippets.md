---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new MessageRule();
requestBody.displayName = "From partner";
requestBody.sequence = 2;
requestBody.isEnabled = true;
requestBody.conditions = new MessageRulePredicates();
requestBody.conditions.senderContains = [
				"adele"
			]
requestBody.actions = new MessageRuleActions();
const recipient = new Recipient();
recipient.additionalData = {
							 ["name" , "Alex Wilbur"],
							 ["address" , "AlexW@contoso.onmicrosoft.com"],
					 }
requestBody.actions.forwardTo = [
				recipient
			]
requestBody.actions.stopProcessingRules = true;
const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messageRules.post(requestBody);
}


```