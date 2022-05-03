---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationClass();
requestBody.description = "Health Level 1";
requestBody.classCode = "Health 501";
requestBody.displayName = "Health 1";
requestBody.externalId = "11019";
requestBody.externalName = "Health Level 1";
requestBody.externalSource = EducationExternalSource.Sis;
requestBody.mailNickname = "fineartschool.net";
const result = async () => {
	await graphServiceClient.education.classes.post(requestBody);
}


```