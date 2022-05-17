---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Contact();
requestBody.givenName = "Pavel";
requestBody.surname = "Bansky";
const emailaddress = new EmailAddress();
emailaddress.additionalData = {
					 "address" : "pavelb@fabrikam.onmicrosoft.com",
					 "name" : "Pavel Bansky"
				 }
requestBody.emailAddresses = [
			emailaddress
		]
requestBody.businessPhones = [
			"+1 732 555 0102"
		]
const result = async () => {
	await graphServiceClient.me.contacts.post(requestBody);
}


```