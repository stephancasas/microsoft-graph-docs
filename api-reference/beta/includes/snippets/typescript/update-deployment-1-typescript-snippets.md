---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Deployment();
requestBody.state = new DeploymentState();
requestBody.state.requestedValue = RequestedDeploymentStateValue.Paused;
requestBody.state.additionalData = {
			 "@odata.type" : "microsoft.graph.windowsUpdates.deploymentState"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.windowsUpdates.deployment"
	 }
const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").patch(requestBody);
}


```