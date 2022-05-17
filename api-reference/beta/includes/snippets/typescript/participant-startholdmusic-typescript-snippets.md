---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new StartHoldMusicRequestBody();
requestBody.customPrompt = new Prompt();
requestBody.customPrompt.additionalData = {
			 "@odata.type" : "#microsoft.graph.mediaPrompt",
				 ["@odata.type" , "#microsoft.graph.mediaInfo"],
				 ["uri" , "https://bot.contoso.com/onHold.wav"],
		 }
requestBody.clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").participantsById("participant-id").startHoldMusic.post(requestBody);
}


```