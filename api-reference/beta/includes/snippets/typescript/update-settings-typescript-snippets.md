---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CaseSettings();
requestBody.redundancyDetection = new RedundancyDetectionSettings();
requestBody.redundancyDetection.isEnabled = false;
requestBody.redundancyDetection.similarityThreshold = 70;
requestBody.redundancyDetection.minWords = 12;
requestBody.redundancyDetection.maxWords = 400000;
requestBody.topicModeling = new TopicModelingSettings();
requestBody.topicModeling.isEnabled = false;
requestBody.topicModeling.ignoreNumbers = false;
requestBody.topicModeling.topicCount = 50;
requestBody.topicModeling.dynamicallyAdjustTopicCount = false;
requestBody.ocr = new OcrSettings();
requestBody.ocr.isEnabled = true;
requestBody.ocr.maxImageSize = 12000;
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").settings.patch(requestBody);
}


```