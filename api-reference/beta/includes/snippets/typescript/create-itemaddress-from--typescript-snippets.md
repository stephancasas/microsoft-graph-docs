---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ItemAddress();
requestBody.displayName = "Home";
requestBody.detail = new PhysicalAddress();
requestBody.detail.type = PhysicalAddressType.Home;
requestBody.detail.postOfficeBox = null,
requestBody.detail.street = "221B Baker Street";
requestBody.detail.city = "London";
requestBody.detail.state = null,
requestBody.detail.countryOrRegion = "United Kingdom";
requestBody.detail.postalCode = "E14 3TD";
const result = async () => {
	await graphServiceClient.me.profile.addresses.post(requestBody);
}


```