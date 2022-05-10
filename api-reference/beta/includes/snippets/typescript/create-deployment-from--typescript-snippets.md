---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Deployment();
requestBody.content = new DeployableContent();
requestBody.content.additionalData = {
			 "@odata.type" : "microsoft.graph.windowsUpdates.featureUpdateReference",
			 "version" : "20H2"
		 }
requestBody.settings = new DeploymentSettings();
requestBody.settings.rollout = new RolloutSettings();
requestBody.settings.rollout.devicesPerOffer = 100;
requestBody.settings.monitoring = new MonitoringSettings();
const monitoringrule = new MonitoringRule();
monitoringrule.additionalData = {
							 "@odata.type" : "#microsoft.graph.windowsUpdates.monitoringRule",
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
	await graphServiceClient.admin.windows.updates.deployments.post(requestBody);
}


```