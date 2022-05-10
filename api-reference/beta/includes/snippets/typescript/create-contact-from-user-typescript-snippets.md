---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Contact();
requestBody.givenName = "Pavel";
requestBody.surname = "Bansky";
const typedemailaddress = new TypedEmailAddress();
typedemailaddress.additionalData = {
					 "address" : "pavelb@contoso.onmicrosoft.com",
					 "name" : "Pavel Bansky",
					 "type" : "personal"
				 }
const typedemailaddress1 = new TypedEmailAddress();
typedemailaddress1.additionalData = {
					 "address" : "pavelb@fabrikam.onmicrosoft.com",
					 "name" : "Pavel Bansky",
					 "type" : "other",
					 "otherLabel" : "Volunteer work"
				 }
requestBody.emailAddresses = [
			typedemailaddress,
			typedemailaddress1
		]
const phone = new Phone();
phone.additionalData = {
					 "number" : "+1 732 555 0102",
					 "type" : "business"
				 }
requestBody.phones = [
			phone
		]
const result = async () => {
	await graphServiceClient.me.contacts.post(requestBody);
}


```