---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonCertification();
requestBody.certificationId = "KB-1235466333663322";
requestBody.description = "Blackbelt in Marketing - Brand Management";
requestBody.displayName = "Marketing Blackbelt - Brand Management";
requestBody.thumbnailUrl = "https://iame.io/dfhdfdfd334.jpg";
requestBody.webUrl = "https://www.iame.io/blackbelt";
const result = async () => {
	await graphServiceClient.me.profile.certifications.post(requestBody);
}


```