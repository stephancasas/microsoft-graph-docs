---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DirectorySetting();
const settingvalue = new SettingValue();
settingvalue.additionalData = {
					 "name" : "CustomBlockedWordsList",
					 "value" : "Contoso"
				 }
requestBody.values = [
			settingvalue
		]
const result = async () => {
	await graphServiceClient.settingsById("directorySetting-id").patch(requestBody);
}


```