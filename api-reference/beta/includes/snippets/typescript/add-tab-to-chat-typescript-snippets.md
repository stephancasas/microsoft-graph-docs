---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamsTab();
requestBody.displayName = "My Contoso Tab";
requestBody.configuration = new TeamsTabConfiguration();
requestBody.configuration.entityId = "2DCA2E6C7A10415CAF6B8AB6661B3154";
requestBody.configuration.contentUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView";
requestBody.configuration.websiteUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154";
requestBody.configuration.removeUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab";
requestBody.additionalData = {
		 "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"
	 }
const result = async () => {
	await graphServiceClient.chatsById("chat-id").tabs.post(requestBody);
}


```