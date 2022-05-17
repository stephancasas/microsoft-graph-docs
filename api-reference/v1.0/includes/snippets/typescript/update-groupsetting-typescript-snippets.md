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
					 "value" : "true"
				 }
requestBody.values = [
			settingvalue
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").settingsById("groupSetting-id").patch(requestBody);
}


```