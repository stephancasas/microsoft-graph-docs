---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GroupSetting();
const settingvalue = new SettingValue();
settingvalue.additionalData = {
					 "name" : "AllowToAddGuests",
					 "value" : "false"
				 }
requestBody.values = [
			settingvalue
		]
const result = async () => {
	await graphServiceClient.groupSettingsById("groupSetting-id").patch(requestBody);
}


```