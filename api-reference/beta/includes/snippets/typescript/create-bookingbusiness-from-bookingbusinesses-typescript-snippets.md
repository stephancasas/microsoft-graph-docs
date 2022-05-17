---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BookingBusiness();
requestBody.displayName = "Fourth Coffee";
requestBody.address = new PhysicalAddress();
requestBody.address.type = PhysicalAddressType.Mall;
requestBody.address.postOfficeBox = "P.O. Box 123";
requestBody.address.street = "4567 Main Street";
requestBody.address.city = "Buffalo";
requestBody.address.state = "NY";
requestBody.address.countryOrRegion = "USA";
requestBody.address.postalCode = "98052";
requestBody.phone = "206-555-0100";
requestBody.email = "manager@fourthcoffee.com";
requestBody.webSiteUrl = "https://www.fourthcoffee.com";
requestBody.defaultCurrencyIso = "USD";
const result = async () => {
	await graphServiceClient.bookingBusinesses.post(requestBody);
}


```