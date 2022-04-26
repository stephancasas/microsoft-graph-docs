---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonAward();
requestBody.description = "Lifetime Achievement award from the International Association of Branding Managers";
requestBody.displayName = "Lifetime Achievement Award For Excellence in Branding";
requestBody.issuedDate = "Date";
requestBody.issuingAuthority = "International Association of Branding Management";
requestBody.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";
requestBody.webUrl = "https://www.iabm.io";
const result = async () => {
	await graphServiceClient.me.profile.awards.post(requestBody);
}


```