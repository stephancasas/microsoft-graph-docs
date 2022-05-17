---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AnswerRequestBody();
requestBody.callbackUri = "https://bot.contoso.com/api/calls";
requestBody.acceptedModalities = [
			"audio"
		]
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = {
			 "@odata.type" : "#microsoft.graph.appHostedMediaConfig",
			 "blob" : "<Media Session Configuration Blob>"
		 }
async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```