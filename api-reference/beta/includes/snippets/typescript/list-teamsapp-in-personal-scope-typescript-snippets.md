---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "appDefinitions($select=id,displayName,allowedInstallationScopes)",
	filter : "appDefinitions/any",
};
const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(requestParameters);
}


```