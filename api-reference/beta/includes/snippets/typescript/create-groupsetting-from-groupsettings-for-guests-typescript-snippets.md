---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DirectorySetting();
requestBody.templateId = "08d542b9-071f-4e16-94b0-74abb372e3d9";
const settingvalue = new SettingValue();
settingvalue.additionalData = {
					 "name" : "AllowToAddGuests",
					 "value" : "false"
				 }
requestBody.values = [
			settingvalue
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").settings.post(requestBody);
}


```