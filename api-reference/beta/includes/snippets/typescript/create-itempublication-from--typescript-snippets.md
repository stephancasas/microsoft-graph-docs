---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ItemPublication();
requestBody.description = "One persons journey to the top of the branding management field.";
requestBody.displayName = "Got Brands? The story of Innocenty Popov and his journey to the top.";
requestBody.publishedDate = "Date";
requestBody.publisher = "International Association of Branding Management Publishing";
requestBody.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";
requestBody.webUrl = "https://www.iabm.io";
const result = async () => {
	await graphServiceClient.me.profile.publications.post(requestBody);
}


```