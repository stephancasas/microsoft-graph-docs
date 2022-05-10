---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new RecordResponseRequestBody();
requestBody.bargeInAllowed = true;
requestBody.clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";
const prompt = new Prompt();
prompt.additionalData = {
					 "@odata.type" : "#microsoft.graph.mediaPrompt",
						 ["uri" , "https://cdn.contoso.com/beep.wav"],
						 ["resourceId" , "1D6DE2D4-CD51-4309-8DAA-70768651088E"],
				 }
requestBody.prompts = [
			prompt
		]
requestBody.maxRecordDurationInSeconds = 10;
requestBody.initialSilenceTimeoutInSeconds = 5;
requestBody.maxSilenceTimeoutInSeconds = 2;
requestBody.playBeep = true;
requestBody.stopTones = [
			"#",
			"1",
			"*"
		]
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").recordResponse.post(requestBody);
}


```