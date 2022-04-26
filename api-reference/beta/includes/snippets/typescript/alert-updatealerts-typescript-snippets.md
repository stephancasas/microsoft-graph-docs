---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdateAlertsRequestBody();
const alert = new Alert();
alert.additionalData = {
					 "assignedTo" : "String",
					 "closedDateTime" : "String (timestamp)",
					 "comments" : [
							"String"
						]
						 ["@odata.type" , "microsoft.graph.alertFeedback"],
					 "id" : "String (identifier)",
						 ["@odata.type" , "microsoft.graph.alertStatus"],
					 "tags" : [
							"String"
						]
						 ["provider" , "String"],
						 ["vendor" , "String"],
				 }
requestBody.value = [
			alert
		]
const result = async () => {
	await graphServiceClient.security.alerts.updateAlerts.post(requestBody);
}


```