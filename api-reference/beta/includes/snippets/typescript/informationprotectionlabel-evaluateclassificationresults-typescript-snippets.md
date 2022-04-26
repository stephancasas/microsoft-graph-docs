---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EvaluateClassificationResultsRequestBody();
requestBody.contentInfo = new ContentInfo();
requestBody.contentInfo.format = ContentFormat.Default;
requestBody.contentInfo.identifier = null,
requestBody.contentInfo.state = ContentState.Rest;
requestBody.contentInfo.additionalData = {
			 "@odata.type" : "#microsoft.graph.contentInfo",
			 "format@odata.type" : "#microsoft.graph.contentFormat",
			 "state@odata.type" : "#microsoft.graph.contentState"
		 }
const classificationresult = new ClassificationResult();
classificationresult.additionalData = {
					 "sensitiveTypeId" : "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
					 "count" : 4,
					 "confidenceLevel" : 75
				 }
requestBody.classificationResults = [
			classificationresult
		]
const headers = {
	"User-Agent": "ContosoLOBApp/1.0",
};
const result = async () => {
	await graphServiceClient.informationProtection.policy.labels.evaluateClassificationResults.post(requestBody, headers);
}


```