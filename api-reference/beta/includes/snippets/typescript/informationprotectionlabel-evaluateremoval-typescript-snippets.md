---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EvaluateRemovalRequestBody();
requestBody.contentInfo = new ContentInfo();
requestBody.contentInfo.format = ContentFormat.Default;
requestBody.contentInfo.identifier = null,
requestBody.contentInfo.state = ContentState.Rest;
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
						 "value" : "True"
					 }
const keyvaluepair1 = new KeyValuePair();
keyvaluepair1.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
						 "value" : "Standard"
					 }
const keyvaluepair2 = new KeyValuePair();
keyvaluepair2.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
						 "value" : "1/1/0001 12:00:00 AM"
					 }
const keyvaluepair3 = new KeyValuePair();
keyvaluepair3.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
						 "value" : "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
					 }
const keyvaluepair4 = new KeyValuePair();
keyvaluepair4.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
						 "value" : "General"
					 }
const keyvaluepair5 = new KeyValuePair();
keyvaluepair5.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
						 "value" : "0"
					 }
const keyvaluepair6 = new KeyValuePair();
keyvaluepair6.additionalData = {
						 "@odata.type" : "#microsoft.graph.keyValuePair",
						 "name" : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
						 "value" : "00000000-0000-0000-0000-000000000000"
					 }
requestBody.contentInfo.metadata = [
				keyvaluepair,
				keyvaluepair1,
				keyvaluepair2,
				keyvaluepair3,
				keyvaluepair4,
				keyvaluepair5,
				keyvaluepair6
			]
requestBody.contentInfo.additionalData = {
			 "@odata.type" : "#microsoft.graph.contentInfo",
			 "format@odata.type" : "#microsoft.graph.contentFormat",
			 "state@odata.type" : "#microsoft.graph.contentState",
			 "metadata@odata.type" : "#Collection(microsoft.graph.keyValuePair)"
		 }
requestBody.downgradeJustification = new DowngradeJustification();
requestBody.downgradeJustification.justificationMessage = "The information has been declassified.";
requestBody.downgradeJustification.isDowngradeJustified = true;
const headers = {
	"User-Agent": "ContosoLOBApp/1.0",
};
const result = async () => {
	await graphServiceClient.informationProtection.policy.labels.evaluateRemoval.post(requestBody, headers);
}


```