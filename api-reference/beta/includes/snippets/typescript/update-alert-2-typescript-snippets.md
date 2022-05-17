---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Alert();
requestBody.assignedTo = "String";
requestBody.closedDateTime =  new Date("String (timestamp)");
requestBody.comments = [
			"String"
		]
requestBody.feedback = AlertFeedback.@odata.type: microsoft.graph.alertFeedback;
requestBody.status = AlertStatus.@odata.type: microsoft.graph.alertStatus;
requestBody.tags = [
			"String"
		]
requestBody.vendorInformation = new SecurityVendorInformation();
requestBody.vendorInformation.provider = "String";
requestBody.vendorInformation.vendor = "String";
const headers = {
	"Prefer": "return=representation",
};
const result = async () => {
	await graphServiceClient.security.alertsById("alert-id").patch(requestBody, headers);
}


```