---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Deployment();
requestBody.settings = new DeploymentSettings();
requestBody.settings.monitoring = new MonitoringSettings();
const monitoringrule = new MonitoringRule();
monitoringrule.additionalData = {
							 "signal" : "rollback",
							 "threshold" : 5,
							 "action" : "pauseDeployment"
						 }
requestBody.settings.monitoring.monitoringRules = [
					monitoringrule
				]
requestBody.settings.additionalData = {
			 "@odata.type" : "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.windowsUpdates.deployment"
	 }
const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").patch(requestBody);
}


```