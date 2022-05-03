---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ThreatAssessmentRequest();
requestBody.expectedAssessment = ThreatExpectedAssessment.Block;
requestBody.category = ThreatCategory.Phishing;
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.urlAssessmentRequest",
		 "url" : "http://test.com"
	 }
const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequests.post(requestBody);
}


```