---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DirectorySetting();
requestBody.templateId = "62375ab9-6b52-47ed-826b-58e47e0e304b";
const settingvalue = new SettingValue();
settingvalue.additionalData = {
					 "name" : "GuestUsageGuidelinesUrl",
					 "value" : "https://privacy.contoso.com/privacystatement"
				 }
const settingvalue1 = new SettingValue();
settingvalue1.additionalData = {
					 "name" : "EnableMSStandardBlockedWords",
					 "value" : "true"
				 }
const settingvalue2 = new SettingValue();
settingvalue2.additionalData = {
					 "name" : "EnableMIPLabels",
					 "value" : "true"
				 }
const settingvalue3 = new SettingValue();
settingvalue3.additionalData = {
					 "name" : "PrefixSuffixNamingRequirement",
					 "value" : "[Contoso-][GroupName]"
				 }
requestBody.values = [
			settingvalue,
			settingvalue1,
			settingvalue2,
			settingvalue3
		]
const result = async () => {
	await graphServiceClient.settings.post(requestBody);
}


```