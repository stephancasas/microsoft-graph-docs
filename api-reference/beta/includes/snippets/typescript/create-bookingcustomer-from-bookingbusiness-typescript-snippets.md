---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BookingCustomer();
requestBody.displayName = "Joni Sherman";
requestBody.emailAddress = "jonis@relecloud.com";
const physicaladdress = new PhysicalAddress();
physicaladdress.additionalData = {
					 "postOfficeBox" : "",
					 "street" : "4567 Main Street",
					 "city" : "Buffalo",
					 "state" : "NY",
					 "countryOrRegion" : "USA",
					 "postalCode" : "98052",
					 "type" : "home"
				 }
const physicaladdress1 = new PhysicalAddress();
physicaladdress1.additionalData = {
					 "postOfficeBox" : "",
					 "street" : "4570 Main Street",
					 "city" : "Buffalo",
					 "state" : "NY",
					 "countryOrRegion" : "USA",
					 "postalCode" : "98054",
					 "type" : "business"
				 }
requestBody.addresses = [
			physicaladdress,
			physicaladdress1
		]
const phone = new Phone();
phone.additionalData = {
					 "number" : "206-555-0100",
					 "type" : "home"
				 }
const phone1 = new Phone();
phone1.additionalData = {
					 "number" : "206-555-0200",
					 "type" : "business"
				 }
requestBody.phones = [
			phone,
			phone1
		]
const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").customers.post(requestBody);
}


```