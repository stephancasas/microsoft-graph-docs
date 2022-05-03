---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ThreatAssessmentRequest();
requestBody.expectedAssessment = ThreatExpectedAssessment.Block;
requestBody.category = ThreatCategory.Malware;
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.emailFileAssessmentRequest",
		 "recipientEmail" : "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
		 "contentData" : "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
	 }
const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequests.post(requestBody);
}


```