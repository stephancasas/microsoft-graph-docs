---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Team();
const channel = new Channel();
channel.additionalData = {
					 "displayName" : "Class Announcements 📢",
					 "isFavoriteByDefault" : true
				 }
const channel1 = new Channel();
channel1.additionalData = {
					 "displayName" : "Homework 🏋️",
					 "isFavoriteByDefault" : true
				 }
requestBody.channels = [
			channel,
			channel1
		]
requestBody.memberSettings = new TeamMemberSettings();
requestBody.memberSettings.allowCreateUpdateChannels = false;
requestBody.memberSettings.allowDeleteChannels = false;
requestBody.memberSettings.allowAddRemoveApps = false;
requestBody.memberSettings.allowCreateUpdateRemoveTabs = false;
requestBody.memberSettings.allowCreateUpdateRemoveConnectors = false;
const teamsappinstallation = new TeamsAppInstallation();
teamsappinstallation.additionalData = {
					 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
				 }
const teamsappinstallation1 = new TeamsAppInstallation();
teamsappinstallation1.additionalData = {
					 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
				 }
requestBody.installedApps = [
			teamsappinstallation,
			teamsappinstallation1
		]
requestBody.additionalData = {
		 "template@odata.bind" : "https://graph.microsoft.com/beta/teamsTemplates('standard')",
		 "group@odata.bind" : "https://graph.microsoft.com/beta/groups('dbd8de4f-5d47-48da-87f1-594bed003375')"
	 }
const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```