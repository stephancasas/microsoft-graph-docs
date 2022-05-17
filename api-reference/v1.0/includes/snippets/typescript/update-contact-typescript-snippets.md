---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Contact();
requestBody.homeAddress = new PhysicalAddress();
requestBody.homeAddress.street = "123 Some street";
requestBody.homeAddress.city = "Seattle";
requestBody.homeAddress.state = "WA";
requestBody.homeAddress.postalCode = "98121";
requestBody.birthday =  new Date("1974-07-22");
const result = async () => {
	await graphServiceClient.me.contactsById("contact-id").patch(requestBody);
}


```