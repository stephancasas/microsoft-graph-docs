---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Contact();
const typedemailaddress = new TypedEmailAddress();
typedemailaddress.additionalData = {
					 "type" : "personal",
					 "name" : "Pavel Bansky",
					 "address" : "pavelb@adatum.onmicrosoft.com"
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
const result = async () => {
	await graphServiceClient.me.contactsById("contact-id").patch(requestBody);
}


```